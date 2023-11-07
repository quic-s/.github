# QUIC-S

## Description

QUIC-S is a continuous file synchronization system based on QUIC protocol. This system is designed to synchronize files between multiple devices, to manage file versions, and to share files with other users.

QUIC-S consists of a server and a client, and the quic-go based quics-protocol is used for communication between the two.

To see server: [quics](https://github.com/quic-s/quics)<br>
To see client: [quics-client](https://github.com/quic-s/quics-client)<br>
To see protocol: [quics-protocol](https://github.com/quic-s/quics-protocol)

## Goal 

The goal of this project is to provide a tool that can be used to synchronize files between two or more computers. The tool should be able to synchronize files in real time, and should be able to handle large files. And most of all, it should be resolved coflict between files by user-self.

#### 1. Real time synchronization

The tool should be able to synchronize files in real time. This means that when a file is changed on one computer, the change should be propagated to the other computers as soon as possible.

#### 2. Large file support

The tool should be able to handle large files. This means that the tool should be able to synchronize files that are several gigabytes in size.

#### 3. Conflict resolution

The tool should be able to resolve conflicts between files. This means that if a file is changed on two computers at the same time, the tool should be able to resolve the conflict by asking the user which version of the file to keep. 

> The standard of time of files is logical time. Logical time is added from 1, when the file have change events. So, the file with the latest logical time is the latest file.

#### 4. History management

The tool should be able to manage the history of files. This means that the tool should be able to keep track of all the changes that have been made to a file, and should be able to revert to a previous version of the file if necessary.

#### 5. Share File

QUIC-S can create links to files synchronized on the server, making it easy to share files with others who are not connected to the system.

## Documentation

For more detail logic and implementation, please check [QUIC-S Docs](https://github.com/quic-s/quics/blob/main/docs/README.md) or each repository's README.md.

## Roadmap

QUIC-S is a program currently under active development, and the development target schedule can be found at [ROADMAP.md](https://github.com/quic-s/quics/blob/main/ROADMAP.md).
