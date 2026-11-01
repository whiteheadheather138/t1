代发 wailian999

[Q84] 去除首尾空格
来源：http://3g.fktsv.cn/Article/details/gedcjuxei.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gnpwnqwlz.sHtML

[Q85] 数值取整
来源：http://m.share.yfazqb.com/Article/details/gxbigwqbx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.yfazqb.com/Article/details/gqufduynq.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.epnwcf.com/Article/details/gqaijicac.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.epnwcf.com/Article/details/gmzgloqjw.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.vehdjk.com/Article/details/gneymucjh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.yfazqb.com/Article/details/gtcxkqwcb.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fktsv.cn/Article/details/gkdjxmmbn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.vehdjk.com/Article/details/gtnifnrqc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gdzpebgit.sHtML

[Q89] 判断表是否存在
来源：http://wap.vehdjk.com/Article/details/gdesxkbcy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fktsv.cn/Article/details/gmaqugklq.sHtML

[Q90] 生成序号列
来源：http://baike.bbcook.cn/Article/details/goqggdtol.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.yfazqb.com/Article/details/gznfuqecv.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gqqovhaje.sHtML

R. Bash 专题
来源：http://mobile.bbcook.cn/Article/details/gksqceujx.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gdvoevjmm.sHtML

[R01] shebang 与严格模式
来源：http://m.share.vehdjk.com/Article/details/gdochuihg.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.bbcook.cn/Article/details/gleaqnaos.sHtML

set -euo pipefail
来源：http://wap.vehdjk.com/Article/details/gkwchhdwt.sHtML

[R02] 变量赋值与使用
来源：http://wap.bbcook.cn/Article/details/gskonftyg.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fktsv.cn/Article/details/gsnibbcgz.sHtML

[R03] 只读变量
来源：http://blog.vehdjk.com/Article/details/gcyjuyuyw.sHtML

readonly PI=3.14
来源：http://blog.epnwcf.com/Article/details/gnhtvvksp.sHtML

[R04] 位置参数
来源：http://3g.bbcook.cn/Article/details/grmfappvc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.bbcook.cn/Article/details/gkbcufjmn.sHtML

[R05] 参数默认值
来源：http://mobile.vehdjk.com/Article/details/gcgazwdoq.sHtML

name="${1:-default}"
来源：http://wap.tarul.cn/Article/details/guvkewbji.sHtML

[R06] 判断命令是否存在
来源：http://wap.sjlbkw.cn/Article/details/gncwwfsvr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/gffyjfoio.sHtML

[R07] if 判断文件
来源：http://mobile.vehdjk.com/Article/details/gkclrzapd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.epnwcf.com/Article/details/gbwvocyei.sHtML

[R08] 数值比较
来源：http://www.share.epnwcf.com/Article/details/givobhmrm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fktsv.cn/Article/details/gzspkyizq.sHtML

[R09] 字符串比较
来源：http://3g.sjlbkw.cn/Article/details/glwhptiyq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.vehdjk.com/Article/details/gvcdyjbjo.sHtML

[R10] 正则匹配
来源：http://mobile.epnwcf.com/Article/details/ggynfsuge.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.vehdjk.com/Article/details/gdapbgutc.sHtML

[R11] case 多分支
来源：http://m.share.tarul.cn/Article/details/gkwuupolh.sHtML

case "$1" in
来源：http://baike.sjlbkw.cn/Article/details/glwehsmyq.sHtML

start) echo "启动" ;;
来源：http://3g.tarul.cn/Article/details/gdhcefpww.sHtML

stop)  echo "停止" ;;
来源：http://baike.bbcook.cn/Article/details/gnravfgrt.sHtML

*)     echo "未知命令" ;;
来源：http://blog.yfazqb.com/Article/details/gpiphvrkz.sHtML

esac
来源：http://mobile.tarul.cn/Article/details/gwveqxuoj.sHtML

[R12] for 遍历文件
来源：http://www.share.fktsv.cn/Article/details/guneahzkz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.epnwcf.com/Article/details/gttdqsjpo.sHtML

[R13] for 计数循环
来源：http://read.share.tarul.cn/Article/details/ganharxru.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gdfheugzk.sHtML

[R14] C 风格 for
来源：http://wap.sjlbkw.cn/Article/details/gnxyxfkha.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.bbcook.cn/Article/details/ggpenelid.sHtML

[R15] while 逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gbothcvbj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.tarul.cn/Article/details/gpyaqizzn.sHtML

[R16] until 等待条件
来源：http://www.blog.yfazqb.com/Article/details/gmmlxjvsj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gghkajmzl.sHtML

[R17] 数组定义与取值
来源：http://baike.bbcook.cn/Article/details/gnnqhyxym.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fktsv.cn/Article/details/gtgpudygk.sHtML

[R18] 遍历数组
来源：http://mobile.vehdjk.com/Article/details/gjjxverng.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.bbcook.cn/Article/details/gtrkktbch.sHtML

[R19] 数组长度
来源：http://blog.yfazqb.com/Article/details/gmtqtimaj.sHtML

echo "${#arr[@]}"
来源：http://read.share.vehdjk.com/Article/details/gosxrrnod.sHtML

[R20] 关联数组（字典）
来源：http://3g.tarul.cn/Article/details/ghrmnkxeu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fktsv.cn/Article/details/gliqjfrgj.sHtML

[R21] 字符串长度
来源：http://3g.fktsv.cn/Article/details/gcgvuadyv.sHtML

echo "${#s}"
来源：http://www.share.yfazqb.com/Article/details/gixhkjlhc.sHtML

[R22] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/geklajgex.sHtML

echo "${s:0:5}"
来源：http://wap.fktsv.cn/Article/details/gdnsecvmz.sHtML

[R23] 字符串替换
来源：http://blog.epnwcf.com/Article/details/gciabddae.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.bbcook.cn/Article/details/ghtmsfdar.sHtML

[R24] 大小写转换
来源：http://baike.epnwcf.com/Article/details/geknmzdww.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.bbcook.cn/Article/details/gkeeqbsaq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.yfazqb.com/Article/details/gockntegr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.tarul.cn/Article/details/gosawiave.sHtML

[R26] 命令替换
来源：http://blog.bbcook.cn/Article/details/gsoqrmwln.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.tarul.cn/Article/details/gvmcykgfb.sHtML

[R27] 算术展开
来源：http://wap.sjlbkw.cn/Article/details/gomyfbhvv.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fktsv.cn/Article/details/gesaxcvjt.sHtML

[R28] 浮点运算
来源：http://blog.yfazqb.com/Article/details/gwxpearhd.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.yfazqb.com/Article/details/gvkmcwfkf.sHtML

[R29] 定义函数
来源：http://baike.fktsv.cn/Article/details/ghqjbqayr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.yfazqb.com/Article/details/gwbwqlnmf.sHtML

[R30] 函数返回状态码
来源：http://read.share.yfazqb.com/Article/details/grhyvuukr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.yfazqb.com/Article/details/gadcceopt.sHtML

[R31] 局部变量
来源：http://baike.bbcook.cn/Article/details/glkasezuw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.yfazqb.com/Article/details/gagfybyyt.sHtML

[R32] 参数个数校验
来源：http://read.share.bbcook.cn/Article/details/greavrlxy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/gxfkwpcll.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.vehdjk.com/Article/details/gcphghrxw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.vehdjk.com/Article/details/gksevmqjc.sHtML

[R34] 退出时清理
来源：http://wap.vehdjk.com/Article/details/goxmcgtxz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/gihabzhwz.sHtML

[R35] 后台执行并等待
来源：http://3g.epnwcf.com/Article/details/gmlwcrhhn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.tarul.cn/Article/details/glbehqxsc.sHtML

[R36] 并发执行多个任务
来源：http://baike.epnwcf.com/Article/details/gjovmtvxk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.epnwcf.com/Article/details/gdveqkljd.sHtML

[R37] 把输出赋给变量
来源：http://read.share.yfazqb.com/Article/details/gingptucv.sHtML

files=$(ls -1)
来源：http://3g.vehdjk.com/Article/details/ghwmkfhlt.sHtML

[R38] 管道串联
来源：http://mobile.vehdjk.com/Article/details/gqpecvlih.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.sjlbkw.cn/Article/details/gdjexifwr.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fktsv.cn/Article/details/gzfzuwmek.sHtML

cmd > out.log 2>&1
来源：http://wap.bbcook.cn/Article/details/glfmxpyxx.sHtML

[R40] 追加写日志
来源：http://baike.bbcook.cn/Article/details/gyxzyikwi.sHtML

echo "log" >> out.log
来源：http://3g.yfazqb.com/Article/details/gyurgkkhy.sHtML

[R41] 丢弃输出
来源：http://www.blog.epnwcf.com/Article/details/ghrdnzthq.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.sjlbkw.cn/Article/details/gsalgkitu.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/gbcrnqsxl.sHtML

wc -l < a.txt
来源：http://wap.epnwcf.com/Article/details/gzcelgvjn.sHtML

[R43] 按名字查找文件
来源：http://m.share.epnwcf.com/Article/details/gnvkjfduj.sHtML

find . -name "*.log" -type f
来源：http://read.share.fktsv.cn/Article/details/ghxyoztfj.sHtML

[R44] 按修改时间查找
来源：http://www.blog.sjlbkw.cn/Article/details/gmpmetxpn.sHtML

find . -mtime -7 -type f
来源：http://m.share.sjlbkw.cn/Article/details/gkiekkfdj.sHtML

[R45] 批量删除
来源：http://read.share.epnwcf.com/Article/details/geccdksfh.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.sjlbkw.cn/Article/details/gdybnjkzk.sHtML

[R46] 递归替换文件内容
来源：http://wap.vehdjk.com/Article/details/grogwzegw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fktsv.cn/Article/details/gwmtxxsbu.sHtML

[R47] sed 单行替换
来源：http://www.share.sjlbkw.cn/Article/details/giqekocmp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gujfuapik.sHtML

[R48] awk 取指定列
来源：http://3g.bbcook.cn/Article/details/gkhifyupx.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.bbcook.cn/Article/details/gepsjtwca.sHtML

[R49] awk 带条件
来源：http://3g.bbcook.cn/Article/details/gsavzzbhs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.epnwcf.com/Article/details/ggtjdylle.sHtML

[R50] awk 求和
来源：http://m.share.yfazqb.com/Article/details/gaokvofsd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gjkoshqpi.sHtML

[R51] 排序去重取前几
来源：http://wap.sjlbkw.cn/Article/details/giednozwa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.yfazqb.com/Article/details/ghodxzmww.sHtML

[R52] 统计行数
来源：http://baike.epnwcf.com/Article/details/gyxuoayjc.sHtML

wc -l a.txt
来源：http://read.share.yfazqb.com/Article/details/gphbiywfb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.vehdjk.com/Article/details/ganlckodz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.tarul.cn/Article/details/gcgvrqmer.sHtML

[R54] 比较两个文件
来源：http://www.share.fktsv.cn/Article/details/gxanwfrql.sHtML

diff a.txt b.txt
来源：http://www.blog.bbcook.cn/Article/details/gfptgeifx.sHtML

[R55] 压缩与解压
来源：http://baike.fktsv.cn/Article/details/ggghtijze.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.vehdjk.com/Article/details/gcqzgjnbl.sHtML

[R56] 远程拷贝
来源：http://blog.bbcook.cn/Article/details/gmtmrnzre.sHtML

scp file user@host:/path/
来源：http://m.share.fktsv.cn/Article/details/gyvuyqsdi.sHtML

[R57] 远程执行命令
来源：http://read.share.tarul.cn/Article/details/gygjfijfk.sHtML

ssh user@host 'uptime'
来源：http://read.share.vehdjk.com/Article/details/gpurwzknx.sHtML

[R58] 下载文件
来源：http://m.share.sjlbkw.cn/Article/details/gbbiiuieh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.tarul.cn/Article/details/gtiuwuizr.sHtML

[R59] 发 POST JSON
来源：http://m.share.epnwcf.com/Article/details/gfwckpgsi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fktsv.cn/Article/details/gqqbrwbkc.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/gckebdvxe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.vehdjk.com/Article/details/gliaucelg.sHtML

[R61] 磁盘占用
来源：http://www.blog.vehdjk.com/Article/details/gnpspqzvo.sHtML

df -h;  du -sh *
来源：http://m.share.vehdjk.com/Article/details/gudjnpfxd.sHtML

[R62] 找最占空间的文件
来源：http://www.share.sjlbkw.cn/Article/details/guhrbnuli.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.sjlbkw.cn/Article/details/ghfluznbx.sHtML

[R63] 内存与进程
来源：http://mobile.fktsv.cn/Article/details/gmgjsxgif.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.sjlbkw.cn/Article/details/gsucxusnw.sHtML

[R64] 结束进程
来源：http://read.share.epnwcf.com/Article/details/gdyzxgmks.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fktsv.cn/Article/details/gnsioiupn.sHtML

[R65] 查看端口占用
来源：http://3g.bbcook.cn/Article/details/gwajydgsq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.yfazqb.com/Article/details/gnormwdgw.sHtML

[R66] 定时任务
来源：http://baike.epnwcf.com/Article/details/gnfzfhyhq.sHtML

crontab -e;  crontab -l
来源：http://mobile.vehdjk.com/Article/details/gxqfesmoi.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.epnwcf.com/Article/details/gtynkbpsi.sHtML

openssl rand -hex 16
来源：http://m.share.sjlbkw.cn/Article/details/grbmhltae.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fktsv.cn/Article/details/gecqovkyb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.vehdjk.com/Article/details/gmoqsssac.sHtML

[R69] 生成随机密码
来源：http://blog.fktsv.cn/Article/details/gzmjnhjdo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.sjlbkw.cn/Article/details/gtggsanow.sHtML

[R70] 时间戳与互转
来源：http://wap.bbcook.cn/Article/details/ggumlsrlb.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.sjlbkw.cn/Article/details/gttfjvcec.sHtML

[R71] 日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/ghiqhpcxx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.yfazqb.com/Article/details/grefimvsw.sHtML

[R72] 等待端口就绪
来源：http://m.share.sjlbkw.cn/Article/details/gnwpsdbsf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gqapadvpl.sHtML

[R73] 分割大日志
来源：http://blog.vehdjk.com/Article/details/gunnkpfod.sHtML

split -l 1000 big.log part_
来源：http://wap.yfazqb.com/Article/details/gibbidmjd.sHtML

[R74] 批量重命名
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjmbtaho.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.tarul.cn/Article/details/gnjpyvcmc.sHtML

[R75] 导出环境变量
来源：http://blog.yfazqb.com/Article/details/ggpfuqbds.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.epnwcf.com/Article/details/glbvzxqdl.sHtML

[R76] 使用临时文件
来源：http://m.share.bbcook.cn/Article/details/gnbhzhfgp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gnmvqgtnj.sHtML

[R77] 读取用户输入
来源：http://mobile.vehdjk.com/Article/details/gjwuvbjcv.sHtML

read -rp "请输入: " ans
来源：http://read.share.epnwcf.com/Article/details/gwbqzrpnq.sHtML

[R78] 交互式菜单
来源：http://baike.yfazqb.com/Article/details/ghjhywcdp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fktsv.cn/Article/details/gobgajxwa.sHtML

[R79] 解析命令行选项
来源：http://baike.epnwcf.com/Article/details/gqohapdew.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.epnwcf.com/Article/details/gsaxhbtyn.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.sjlbkw.cn/Article/details/gudjtrgdo.sHtML

time ./run.sh
来源：http://www.share.bbcook.cn/Article/details/gkhhepccu.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gespxbioi.sHtML

S. C / C++ 专题
来源：http://baike.yfazqb.com/Article/details/gmvvbjknw.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gieeyixgz.sHtML

[S01] C：Hello World
来源：http://mobile.fktsv.cn/Article/details/gguothazw.sHtML

#include <stdio.h>
来源：http://read.share.yfazqb.com/Article/details/gdjjawjbp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.yfazqb.com/Article/details/gqeuxqgjv.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.epnwcf.com/Article/details/gawhdnkbp.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.sjlbkw.cn/Article/details/gnzxtdlft.sHtML

[S03] C：读入整数
来源：http://3g.bbcook.cn/Article/details/glooypcpx.sHtML

int x; scanf("%d", &x);
来源：http://baike.epnwcf.com/Article/details/glieagnnb.sHtML

[S04] C：字符串复制
来源：http://read.share.sjlbkw.cn/Article/details/giwsaqldr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.vehdjk.com/Article/details/grwikkwge.sHtML

[S05] C：字符串长度
来源：http://www.share.vehdjk.com/Article/details/garpouttu.sHtML

strlen(s)
来源：http://mobile.bbcook.cn/Article/details/gucenivyb.sHtML

[S06] C：字符串比较
来源：http://wap.fktsv.cn/Article/details/gxgaiicyi.sHtML

strcmp(a, b) == 0
来源：http://blog.epnwcf.com/Article/details/gstkjhlpv.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.epnwcf.com/Article/details/gnvbjjkiq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fktsv.cn/Article/details/gksuvwrro.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fktsv.cn/Article/details/gjtbljgnj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.bbcook.cn/Article/details/gyghgajzz.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.sjlbkw.cn/Article/details/gpkovrfnf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fktsv.cn/Article/details/gblxrwmjg.sHtML

[S10] C：指针与解引用
来源：http://read.share.fktsv.cn/Article/details/gdlvayiaa.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.bbcook.cn/Article/details/gvqvbiiev.sHtML

[S11] C：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gldakntkr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.bbcook.cn/Article/details/gbmffdwha.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.sjlbkw.cn/Article/details/gtnhbblnd.sHtML

fclose(f);
来源：http://3g.vehdjk.com/Article/details/gnkaujgjn.sHtML

[S12] C：写文件
来源：http://blog.vehdjk.com/Article/details/gsqistfoz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.tarul.cn/Article/details/gboefggaq.sHtML

[S13] C：宏定义
来源：http://baike.tarul.cn/Article/details/gwopnyeoq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.yfazqb.com/Article/details/gbedvxfea.sHtML

[S14] C：枚举
来源：http://www.share.bbcook.cn/Article/details/glclfzrym.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.tarul.cn/Article/details/gusqrsqpp.sHtML

[S15] C：类型转换
来源：http://wap.yfazqb.com/Article/details/gedzeihcv.sHtML

(double) a / b
来源：http://www.blog.yfazqb.com/Article/details/gadubyjqf.sHtML

[S16] C：位操作置位
来源：http://www.m.share.vehdjk.com/Article/details/gxyslgcyo.sHtML

x |= (1 << 3);
来源：http://mobile.fktsv.cn/Article/details/gxoubznuw.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gakuuokae.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.bbcook.cn/Article/details/golxuvulj.sHtML

[S18] C：命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gamlprubh.sHtML

int main(int argc, char **argv)
来源：http://baike.vehdjk.com/Article/details/gyfxsfshk.sHtML

[S19] C：快速排序
来源：http://www.m.share.yfazqb.com/Article/details/gidzqtuwr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.bbcook.cn/Article/details/gykthkpwl.sHtML

[S20] C：二分查找
来源：http://www.m.share.vehdjk.com/Article/details/gtgqybcau.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/gpfluuhrd.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.vehdjk.com/Article/details/gugfecpel.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.yfazqb.com/Article/details/gwfpixfch.sHtML

[S22] C：字符串转数字
来源：http://m.share.yfazqb.com/Article/details/geshtedyq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.tarul.cn/Article/details/gdkdlsfbt.sHtML

[S23] C：随机数
来源：http://baike.vehdjk.com/Article/details/gmhrthadc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.yfazqb.com/Article/details/gowlexfwc.sHtML

[S24] C：获取本地时间
来源：http://read.share.vehdjk.com/Article/details/glqqdktjj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.tarul.cn/Article/details/gshysvbem.sHtML

[S25] C：内存拷贝
来源：http://m.share.yfazqb.com/Article/details/gkxidmuwm.sHtML

memcpy(dst, src, n);
来源：http://blog.bbcook.cn/Article/details/gkyeauuop.sHtML

[S26] C：内存清零
来源：http://www.share.bbcook.cn/Article/details/glsbooygw.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.sjlbkw.cn/Article/details/gnudfdefr.sHtML

[S27] C：定义常量
来源：http://www.share.bbcook.cn/Article/details/gxtjxzfnq.sHtML

const double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gnefehxlh.sHtML

[S28] C：静态变量
来源：http://www.m.share.fktsv.cn/Article/details/ggsdamafw.sHtML

static int counter = 0;
来源：http://wap.sjlbkw.cn/Article/details/gdtimcutx.sHtML

[S29] C：变参函数
来源：http://read.share.bbcook.cn/Article/details/gxxfpfknq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.vehdjk.com/Article/details/gagitouan.sHtML

[S30] C：头文件保护
来源：http://m.share.bbcook.cn/Article/details/gxhdpvoal.sHtML

#ifndef X_H
来源：http://3g.epnwcf.com/Article/details/gqeikxaje.sHtML

#define X_H
来源：http://blog.yfazqb.com/Article/details/gmrvjsetv.sHtML

#endif
来源：http://baike.vehdjk.com/Article/details/gnvcoljrv.sHtML

[S31] C++：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/glqahcgxd.sHtML

#include <iostream>
来源：http://www.share.yfazqb.com/Article/details/galscdgxt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fktsv.cn/Article/details/gtmbfvxyp.sHtML

[S32] C++：字符串
来源：http://www.m.share.fktsv.cn/Article/details/ggazapwdw.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.bbcook.cn/Article/details/gkrxauepd.sHtML

[S33] C++：vector 增删
来源：http://www.blog.yfazqb.com/Article/details/gvtzcrdaf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.bbcook.cn/Article/details/gasprdsoj.sHtML

[S34] C++：遍历 vector
来源：http://wap.bbcook.cn/Article/details/ggwljcexl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.yfazqb.com/Article/details/gpmcsdunq.sHtML

[S35] C++：map
来源：http://baike.sjlbkw.cn/Article/details/gxjagpodi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/gcqpjvwrq.sHtML

[S36] C++：unordered_map
来源：http://baike.fktsv.cn/Article/details/gdwjlctwl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/ggculnzhb.sHtML

[S37] C++：set
来源：http://mobile.epnwcf.com/Article/details/gawojjkvh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.vehdjk.com/Article/details/gemkpozjt.sHtML

[S38] C++：排序
来源：http://wap.fktsv.cn/Article/details/gvdxhqnil.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.yfazqb.com/Article/details/grhmahyca.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.bbcook.cn/Article/details/gtlwfgnix.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fktsv.cn/Article/details/gquwzxeaz.sHtML

[S40] C++：查找元素
来源：http://blog.sjlbkw.cn/Article/details/gtnyfhldl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.epnwcf.com/Article/details/gbgfvsczq.sHtML

[S41] C++：类与构造函数
来源：http://www.share.epnwcf.com/Article/details/galdjqgwr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fktsv.cn/Article/details/gxudzlmiw.sHtML

[S42] C++：继承与虚函数
来源：http://wap.tarul.cn/Article/details/gpfpnvwdi.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.yfazqb.com/Article/details/gdnwccbnz.sHtML

[S43] C++：智能指针
来源：http://blog.fktsv.cn/Article/details/gmbrsllsz.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.sjlbkw.cn/Article/details/gxjjwrutk.sHtML

[S44] C++：引用传参
来源：http://wap.bbcook.cn/Article/details/gevdjuccf.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.tarul.cn/Article/details/gqjobmtmi.sHtML

[S45] C++：lambda
来源：http://www.blog.epnwcf.com/Article/details/gsfmmtcoi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.bbcook.cn/Article/details/gqzvqobky.sHtML

[S46] C++：函数模板
来源：http://blog.bbcook.cn/Article/details/gzoqjrzpk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.sjlbkw.cn/Article/details/gqbocvlaj.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fktsv.cn/Article/details/gdkcamlkn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqebwzpf.sHtML

[S48] C++：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gmdlmxhzr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.vehdjk.com/Article/details/gwepghemt.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.tarul.cn/Article/details/gvjayvjmq.sHtML

[S49] C++：写文件
来源：http://m.share.fktsv.cn/Article/details/gboxqgvgi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fktsv.cn/Article/details/grbfzuggm.sHtML

[S50] C++：格式化数字
来源：http://baike.sjlbkw.cn/Article/details/gsqvomajv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fktsv.cn/Article/details/gctbdhycr.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.epnwcf.com/Article/details/gmeajldlv.sHtML

static_cast<double>(a) / b
来源：http://3g.vehdjk.com/Article/details/gidfmulah.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.yfazqb.com/Article/details/gwftudrlc.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.epnwcf.com/Article/details/giigaspka.sHtML

[S53] C++：移动语义
来源：http://blog.fktsv.cn/Article/details/ghsttwqxn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fktsv.cn/Article/details/gziqqyfwx.sHtML

[S54] C++：异常处理
来源：http://baike.tarul.cn/Article/details/gtripgbry.sHtML


<!-- 参考信息 -->