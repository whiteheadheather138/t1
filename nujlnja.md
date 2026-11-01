代发 wailian999

[Q86] 读取 JSON 字段
来源：http://mobile.tarul.cn/Article/details/griincbhm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.bbcook.cn/Article/details/gxljlqbne.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.yfazqb.com/Article/details/gdtxggdbo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.bbcook.cn/Article/details/gyotfjhif.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.bbcook.cn/Article/details/gpdhzwndv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fktsv.cn/Article/details/gsoydecng.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.epnwcf.com/Article/details/gopnmssvw.sHtML

[Q89] 判断表是否存在
来源：http://mobile.yfazqb.com/Article/details/gcichlumd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.yfazqb.com/Article/details/gsrzzfkal.sHtML

[Q90] 生成序号列
来源：http://3g.tarul.cn/Article/details/gpcrgypjt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.yfazqb.com/Article/details/gpcrvluem.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gsqknxeoi.sHtML

R. Bash 专题
来源：http://wap.epnwcf.com/Article/details/gpjdfmxwu.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxfhpolee.sHtML

[R01] shebang 与严格模式
来源：http://wap.fktsv.cn/Article/details/glbhlnoqv.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.tarul.cn/Article/details/gsjejrrhr.sHtML

set -euo pipefail
来源：http://www.blog.yfazqb.com/Article/details/giacjqisn.sHtML

[R02] 变量赋值与使用
来源：http://wap.vehdjk.com/Article/details/ghqwzifng.sHtML

name="Tom"; echo "$name"
来源：http://blog.sjlbkw.cn/Article/details/gfhivcwrt.sHtML

[R03] 只读变量
来源：http://wap.tarul.cn/Article/details/gonlpdqkg.sHtML

readonly PI=3.14
来源：http://baike.vehdjk.com/Article/details/genacwbup.sHtML

[R04] 位置参数
来源：http://mobile.epnwcf.com/Article/details/gjtkfauow.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.bbcook.cn/Article/details/gxlptyhjr.sHtML

[R05] 参数默认值
来源：http://m.share.bbcook.cn/Article/details/gllbawlcy.sHtML

name="${1:-default}"
来源：http://baike.sjlbkw.cn/Article/details/gbmanjkpg.sHtML

[R06] 判断命令是否存在
来源：http://baike.epnwcf.com/Article/details/gfpgwtwdc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/ggihgnodk.sHtML

[R07] if 判断文件
来源：http://3g.epnwcf.com/Article/details/gzewfoelm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.tarul.cn/Article/details/gselmdtko.sHtML

[R08] 数值比较
来源：http://www.share.bbcook.cn/Article/details/gorpbuffk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gwocpzqce.sHtML

[R09] 字符串比较
来源：http://wap.vehdjk.com/Article/details/gemrrnfwb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gttfajohr.sHtML

[R10] 正则匹配
来源：http://www.blog.yfazqb.com/Article/details/gwekrefob.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fktsv.cn/Article/details/glqbvfgof.sHtML

[R11] case 多分支
来源：http://www.m.share.epnwcf.com/Article/details/gfrevifvv.sHtML

case "$1" in
来源：http://baike.yfazqb.com/Article/details/gddywisfu.sHtML

start) echo "启动" ;;
来源：http://baike.epnwcf.com/Article/details/gcqokxkqu.sHtML

stop)  echo "停止" ;;
来源：http://wap.bbcook.cn/Article/details/gnxgpnwwv.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.sjlbkw.cn/Article/details/guwslnnxk.sHtML

esac
来源：http://www.share.sjlbkw.cn/Article/details/gezzfjwix.sHtML

[R12] for 遍历文件
来源：http://www.share.tarul.cn/Article/details/grmlqifqf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.tarul.cn/Article/details/gpfywowag.sHtML

[R13] for 计数循环
来源：http://wap.epnwcf.com/Article/details/giyiqhzsq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/gwnekcqof.sHtML

[R14] C 风格 for
来源：http://read.share.yfazqb.com/Article/details/gnpdqbmsy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gtkvojkfv.sHtML

[R15] while 逐行读文件
来源：http://3g.fktsv.cn/Article/details/gbaewnszo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.sjlbkw.cn/Article/details/gioforlod.sHtML

[R16] until 等待条件
来源：http://mobile.bbcook.cn/Article/details/ghyuhbtqn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/gevrklesz.sHtML

[R17] 数组定义与取值
来源：http://read.share.yfazqb.com/Article/details/gnioihisd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fktsv.cn/Article/details/gnxiizoth.sHtML

[R18] 遍历数组
来源：http://wap.epnwcf.com/Article/details/gjptsvurd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.tarul.cn/Article/details/ggkrpwbqx.sHtML

[R19] 数组长度
来源：http://3g.fktsv.cn/Article/details/gomldjnjx.sHtML

echo "${#arr[@]}"
来源：http://baike.tarul.cn/Article/details/gzzkeudnm.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.vehdjk.com/Article/details/ghmhxyxmc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fktsv.cn/Article/details/geztbrhdc.sHtML

[R21] 字符串长度
来源：http://www.share.fktsv.cn/Article/details/gwkmldejp.sHtML

echo "${#s}"
来源：http://www.share.yfazqb.com/Article/details/gnxidxazb.sHtML

[R22] 截取子串
来源：http://www.share.tarul.cn/Article/details/gnectkpqk.sHtML

echo "${s:0:5}"
来源：http://3g.vehdjk.com/Article/details/gwmvvztnx.sHtML

[R23] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gwinljvmb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.yfazqb.com/Article/details/gvxyelvtp.sHtML

[R24] 大小写转换
来源：http://baike.sjlbkw.cn/Article/details/gywoszbpv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.sjlbkw.cn/Article/details/gkdwzfvkf.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.epnwcf.com/Article/details/gmqzxzmnd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.tarul.cn/Article/details/glfwdqcal.sHtML

[R26] 命令替换
来源：http://www.m.share.tarul.cn/Article/details/gnrygjwon.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.yfazqb.com/Article/details/gvonffmhp.sHtML

[R27] 算术展开
来源：http://3g.yfazqb.com/Article/details/gzlksabiv.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fktsv.cn/Article/details/gcfzlxlzc.sHtML

[R28] 浮点运算
来源：http://baike.bbcook.cn/Article/details/gpvineesv.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.epnwcf.com/Article/details/gfwctkqfh.sHtML

[R29] 定义函数
来源：http://wap.bbcook.cn/Article/details/gjewliuht.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.epnwcf.com/Article/details/glprlngvb.sHtML

[R30] 函数返回状态码
来源：http://wap.bbcook.cn/Article/details/gdjrkzbio.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.sjlbkw.cn/Article/details/gcayabdvj.sHtML

[R31] 局部变量
来源：http://baike.epnwcf.com/Article/details/guvsgkqxv.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fktsv.cn/Article/details/gpvsgfbwq.sHtML

[R32] 参数个数校验
来源：http://wap.vehdjk.com/Article/details/giaarpohh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/garkxytic.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.tarul.cn/Article/details/ghgztguti.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.sjlbkw.cn/Article/details/gtwqhxpyq.sHtML

[R34] 退出时清理
来源：http://baike.sjlbkw.cn/Article/details/gzqiilhhc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/gdegapmuo.sHtML

[R35] 后台执行并等待
来源：http://www.share.bbcook.cn/Article/details/gvbskdurt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.yfazqb.com/Article/details/gsenpqdkv.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.vehdjk.com/Article/details/gidxffclo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.epnwcf.com/Article/details/gapllqqoa.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fktsv.cn/Article/details/guahocrwa.sHtML

files=$(ls -1)
来源：http://baike.fktsv.cn/Article/details/gevfbipij.sHtML

[R38] 管道串联
来源：http://wap.yfazqb.com/Article/details/gvpcgvrdo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.bbcook.cn/Article/details/gyngofgoy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.vehdjk.com/Article/details/gqtfvedsk.sHtML

cmd > out.log 2>&1
来源：http://mobile.sjlbkw.cn/Article/details/ghkhrmlpm.sHtML

[R40] 追加写日志
来源：http://www.m.share.fktsv.cn/Article/details/gzvzqhoda.sHtML

echo "log" >> out.log
来源：http://baike.bbcook.cn/Article/details/gyggetbxm.sHtML

[R41] 丢弃输出
来源：http://baike.epnwcf.com/Article/details/gwxuqpoyi.sHtML

cmd >/dev/null 2>&1
来源：http://baike.yfazqb.com/Article/details/ghdwxhsmv.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/gsaexpsyh.sHtML

wc -l < a.txt
来源：http://m.share.vehdjk.com/Article/details/gwvvqctnn.sHtML

[R43] 按名字查找文件
来源：http://3g.yfazqb.com/Article/details/grwraesnk.sHtML

find . -name "*.log" -type f
来源：http://wap.yfazqb.com/Article/details/geobuwwvv.sHtML

[R44] 按修改时间查找
来源：http://read.share.tarul.cn/Article/details/gfbwrwxsv.sHtML

find . -mtime -7 -type f
来源：http://m.share.tarul.cn/Article/details/gruxpsllx.sHtML

[R45] 批量删除
来源：http://www.blog.epnwcf.com/Article/details/giqowjosk.sHtML

find . -name "*.tmp" -delete
来源：http://blog.bbcook.cn/Article/details/gjviroijq.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.yfazqb.com/Article/details/gvyrofypm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.sjlbkw.cn/Article/details/glmmqejtu.sHtML

[R47] sed 单行替换
来源：http://blog.fktsv.cn/Article/details/gxaypofxn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.yfazqb.com/Article/details/gnmvloblu.sHtML

[R48] awk 取指定列
来源：http://3g.epnwcf.com/Article/details/gaaxppfgt.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.bbcook.cn/Article/details/gdwafvwqj.sHtML

[R49] awk 带条件
来源：http://3g.yfazqb.com/Article/details/glhnuyjnz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.bbcook.cn/Article/details/ghweohwkw.sHtML

[R50] awk 求和
来源：http://www.blog.bbcook.cn/Article/details/gtodepood.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.tarul.cn/Article/details/gvetevqnf.sHtML

[R51] 排序去重取前几
来源：http://mobile.tarul.cn/Article/details/glzmmpksi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fktsv.cn/Article/details/gacknsgdn.sHtML

[R52] 统计行数
来源：http://www.blog.fktsv.cn/Article/details/glgvottpb.sHtML

wc -l a.txt
来源：http://3g.fktsv.cn/Article/details/gramzvdli.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.vehdjk.com/Article/details/gpcbyysnb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.epnwcf.com/Article/details/gpehgfgjl.sHtML

[R54] 比较两个文件
来源：http://baike.yfazqb.com/Article/details/gcclwcqit.sHtML

diff a.txt b.txt
来源：http://www.m.share.vehdjk.com/Article/details/gggabtgjz.sHtML

[R55] 压缩与解压
来源：http://3g.bbcook.cn/Article/details/grgkmeequ.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.sjlbkw.cn/Article/details/gtdjioadz.sHtML

[R56] 远程拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gyvuoqaau.sHtML

scp file user@host:/path/
来源：http://mobile.vehdjk.com/Article/details/ghgwllwgo.sHtML

[R57] 远程执行命令
来源：http://baike.vehdjk.com/Article/details/gfztsncmq.sHtML

ssh user@host 'uptime'
来源：http://www.blog.epnwcf.com/Article/details/gjdqxaepz.sHtML

[R58] 下载文件
来源：http://baike.yfazqb.com/Article/details/gnapcnuhc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fktsv.cn/Article/details/gdlqjwfev.sHtML

[R59] 发 POST JSON
来源：http://read.share.tarul.cn/Article/details/gejsrkslp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.yfazqb.com/Article/details/gwxquhlfg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/gsvlmftev.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.epnwcf.com/Article/details/gkmctjbyz.sHtML

[R61] 磁盘占用
来源：http://m.share.vehdjk.com/Article/details/gccwdoegb.sHtML

df -h;  du -sh *
来源：http://www.blog.sjlbkw.cn/Article/details/glhdoeoib.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fktsv.cn/Article/details/ggniqrruv.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.epnwcf.com/Article/details/gtwcystbx.sHtML

[R63] 内存与进程
来源：http://mobile.vehdjk.com/Article/details/guedsvvka.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fktsv.cn/Article/details/gbdhqsfbv.sHtML

[R64] 结束进程
来源：http://mobile.bbcook.cn/Article/details/grkxkevcm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.bbcook.cn/Article/details/glijtfvss.sHtML

[R65] 查看端口占用
来源：http://www.blog.fktsv.cn/Article/details/gsjnmmykt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.epnwcf.com/Article/details/ghdlrfpvv.sHtML

[R66] 定时任务
来源：http://3g.bbcook.cn/Article/details/gdfnuuqxy.sHtML

crontab -e;  crontab -l
来源：http://baike.fktsv.cn/Article/details/gundusgqm.sHtML

[R67] 生成随机十六进制串
来源：http://3g.bbcook.cn/Article/details/gosjfhpsr.sHtML

openssl rand -hex 16
来源：http://mobile.bbcook.cn/Article/details/gpscectab.sHtML

[R68] 计算文件校验值
来源：http://3g.sjlbkw.cn/Article/details/ggzmkdfyf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fktsv.cn/Article/details/gibeknbjb.sHtML

[R69] 生成随机密码
来源：http://www.blog.yfazqb.com/Article/details/gwawuussx.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fktsv.cn/Article/details/gkcugfdxc.sHtML

[R70] 时间戳与互转
来源：http://mobile.sjlbkw.cn/Article/details/gaqqbuakc.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.yfazqb.com/Article/details/gajdrykfb.sHtML

[R71] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gvejiqaqa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.epnwcf.com/Article/details/gtueubuon.sHtML

[R72] 等待端口就绪
来源：http://blog.epnwcf.com/Article/details/gxjnpqrsr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/grjrcoatu.sHtML

[R73] 分割大日志
来源：http://mobile.vehdjk.com/Article/details/gvewqopjc.sHtML

split -l 1000 big.log part_
来源：http://m.share.bbcook.cn/Article/details/gwjyolkph.sHtML

[R74] 批量重命名
来源：http://mobile.epnwcf.com/Article/details/glonqaztw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.yfazqb.com/Article/details/grxlexfcj.sHtML

[R75] 导出环境变量
来源：http://wap.epnwcf.com/Article/details/gahxzoqkv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.yfazqb.com/Article/details/gahtkliyk.sHtML

[R76] 使用临时文件
来源：http://wap.tarul.cn/Article/details/gofkurnua.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.epnwcf.com/Article/details/gbjnzvijx.sHtML

[R77] 读取用户输入
来源：http://www.blog.epnwcf.com/Article/details/grpkmddlq.sHtML

read -rp "请输入: " ans
来源：http://read.share.sjlbkw.cn/Article/details/gftrzwyuj.sHtML

[R78] 交互式菜单
来源：http://www.share.sjlbkw.cn/Article/details/gduhmieqj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.sjlbkw.cn/Article/details/gadqptesv.sHtML

[R79] 解析命令行选项
来源：http://read.share.sjlbkw.cn/Article/details/gfrmzkwse.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.sjlbkw.cn/Article/details/ggqujpfxp.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.vehdjk.com/Article/details/gxqtygpod.sHtML

time ./run.sh
来源：http://blog.sjlbkw.cn/Article/details/ggnfnazwj.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gqnrjhdyv.sHtML

S. C / C++ 专题
来源：http://wap.tarul.cn/Article/details/gllsoktzb.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gvuqmfrkh.sHtML

[S01] C：Hello World
来源：http://3g.bbcook.cn/Article/details/gsbsytrmn.sHtML

#include <stdio.h>
来源：http://read.share.fktsv.cn/Article/details/ghhqzwgyb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.tarul.cn/Article/details/gqmntaxao.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/gpdmnlgpa.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.tarul.cn/Article/details/gbszcwipk.sHtML

[S03] C：读入整数
来源：http://m.share.bbcook.cn/Article/details/govuobeic.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.vehdjk.com/Article/details/gsajxepib.sHtML

[S04] C：字符串复制
来源：http://m.share.sjlbkw.cn/Article/details/gybkokewb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.sjlbkw.cn/Article/details/ggonmlntp.sHtML

[S05] C：字符串长度
来源：http://blog.bbcook.cn/Article/details/gpdirrpzz.sHtML

strlen(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/geabhghpk.sHtML

[S06] C：字符串比较
来源：http://wap.sjlbkw.cn/Article/details/gcpgstahi.sHtML

strcmp(a, b) == 0
来源：http://baike.epnwcf.com/Article/details/gxwazkljp.sHtML

[S07] C：数组遍历求和
来源：http://3g.tarul.cn/Article/details/griommfgq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.tarul.cn/Article/details/giyobbfvd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fktsv.cn/Article/details/gkydfcdjv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.tarul.cn/Article/details/gycowjtxa.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.tarul.cn/Article/details/gdivlogjo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.yfazqb.com/Article/details/gbfkzokhd.sHtML

[S10] C：指针与解引用
来源：http://3g.fktsv.cn/Article/details/gernihbgc.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fktsv.cn/Article/details/glzicyyki.sHtML

[S11] C：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gtyffyqba.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.vehdjk.com/Article/details/glvzktuyr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fktsv.cn/Article/details/gbvucpxyw.sHtML

fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gwtksjtgq.sHtML

[S12] C：写文件
来源：http://baike.fktsv.cn/Article/details/gaowrolxi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/gboctdblc.sHtML

[S13] C：宏定义
来源：http://www.blog.fktsv.cn/Article/details/grtelxrsk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.sjlbkw.cn/Article/details/gihzffxjy.sHtML

[S14] C：枚举
来源：http://www.blog.fktsv.cn/Article/details/gxhijoycp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fktsv.cn/Article/details/gktkpbyyx.sHtML

[S15] C：类型转换
来源：http://mobile.epnwcf.com/Article/details/gbvfsqhbf.sHtML

(double) a / b
来源：http://wap.yfazqb.com/Article/details/guwiixlep.sHtML

[S16] C：位操作置位
来源：http://3g.fktsv.cn/Article/details/gudigpkeu.sHtML

x |= (1 << 3);
来源：http://m.share.epnwcf.com/Article/details/gfowjhbsv.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gjalmzjve.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.yfazqb.com/Article/details/gzvnnozkc.sHtML

[S18] C：命令行参数
来源：http://www.m.share.tarul.cn/Article/details/gwdewdsdx.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.epnwcf.com/Article/details/gfzczaehb.sHtML

[S19] C：快速排序
来源：http://3g.epnwcf.com/Article/details/gnxuckxjt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/gioelmcvf.sHtML

[S20] C：二分查找
来源：http://www.blog.epnwcf.com/Article/details/ggsxurqgr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.tarul.cn/Article/details/gvzemrudk.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdhoicec.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.yfazqb.com/Article/details/ghtmujpok.sHtML

[S22] C：字符串转数字
来源：http://wap.bbcook.cn/Article/details/gmbjzvbuz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.epnwcf.com/Article/details/gxujljlax.sHtML

[S23] C：随机数
来源：http://wap.bbcook.cn/Article/details/guhqdabkx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.epnwcf.com/Article/details/ggfohjjix.sHtML

[S24] C：获取本地时间
来源：http://wap.fktsv.cn/Article/details/gdhjqjbnb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fktsv.cn/Article/details/gileawhmf.sHtML

[S25] C：内存拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gilnlxark.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.epnwcf.com/Article/details/grwwezbmt.sHtML

[S26] C：内存清零
来源：http://www.share.fktsv.cn/Article/details/gcntmvtfu.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fktsv.cn/Article/details/ghtxvbbvy.sHtML

[S27] C：定义常量
来源：http://3g.epnwcf.com/Article/details/ghctiuqnu.sHtML

const double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gekzqeoas.sHtML

[S28] C：静态变量
来源：http://www.share.sjlbkw.cn/Article/details/ggzvirush.sHtML

static int counter = 0;
来源：http://www.blog.tarul.cn/Article/details/gmjsfybeq.sHtML

[S29] C：变参函数
来源：http://baike.vehdjk.com/Article/details/gplrruxac.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.sjlbkw.cn/Article/details/gqxeqxbtl.sHtML

[S30] C：头文件保护
来源：http://blog.yfazqb.com/Article/details/gghsoicrq.sHtML

#ifndef X_H
来源：http://m.share.sjlbkw.cn/Article/details/gflwxsecx.sHtML

#define X_H
来源：http://read.share.fktsv.cn/Article/details/goynorlyy.sHtML

#endif
来源：http://baike.sjlbkw.cn/Article/details/gnqyrhqsx.sHtML

[S31] C++：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gfvzuezyx.sHtML

#include <iostream>
来源：http://www.m.share.yfazqb.com/Article/details/gksuxoriy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.yfazqb.com/Article/details/ggtqzftir.sHtML

[S32] C++：字符串
来源：http://3g.bbcook.cn/Article/details/gaawyfcre.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.yfazqb.com/Article/details/gaiylydib.sHtML

[S33] C++：vector 增删
来源：http://3g.epnwcf.com/Article/details/gzzdsebvn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.bbcook.cn/Article/details/gmwpdnhzp.sHtML

[S34] C++：遍历 vector
来源：http://blog.epnwcf.com/Article/details/gtfinwvqj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fktsv.cn/Article/details/gccmddhoy.sHtML

[S35] C++：map
来源：http://www.m.share.yfazqb.com/Article/details/gmzlijcjf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.tarul.cn/Article/details/gsjvhcvhz.sHtML

[S36] C++：unordered_map
来源：http://blog.fktsv.cn/Article/details/geqtloecy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/grekchqmm.sHtML

[S37] C++：set
来源：http://m.share.yfazqb.com/Article/details/gqbylaqdx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.yfazqb.com/Article/details/gzrtqvvua.sHtML

[S38] C++：排序
来源：http://www.share.epnwcf.com/Article/details/ggaaxsafd.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.epnwcf.com/Article/details/gklvqtgqk.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.bbcook.cn/Article/details/gowkzdenx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fktsv.cn/Article/details/gbwobdmds.sHtML

[S40] C++：查找元素
来源：http://read.share.fktsv.cn/Article/details/gkhednetq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.epnwcf.com/Article/details/glgeteziu.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gfxvczljb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.epnwcf.com/Article/details/gsfnqlarg.sHtML

[S42] C++：继承与虚函数
来源：http://wap.bbcook.cn/Article/details/gskavttzq.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.sjlbkw.cn/Article/details/gozoyqtsq.sHtML

[S43] C++：智能指针
来源：http://mobile.fktsv.cn/Article/details/ghrntzxuk.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.yfazqb.com/Article/details/ghlmvdata.sHtML

[S44] C++：引用传参
来源：http://mobile.vehdjk.com/Article/details/gfrobxszk.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fktsv.cn/Article/details/gizraqrko.sHtML

[S45] C++：lambda
来源：http://baike.yfazqb.com/Article/details/guxzkiufz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.vehdjk.com/Article/details/gktdqgrkc.sHtML

[S46] C++：函数模板
来源：http://read.share.vehdjk.com/Article/details/gdfyegahs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.yfazqb.com/Article/details/gssnvbazv.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.yfazqb.com/Article/details/gagbocgbf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.sjlbkw.cn/Article/details/gkkskqard.sHtML

[S48] C++：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/glvgszird.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.vehdjk.com/Article/details/gjnbzwyvb.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.yfazqb.com/Article/details/glpjkwtit.sHtML

[S49] C++：写文件
来源：http://blog.epnwcf.com/Article/details/gtqmgvphr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.tarul.cn/Article/details/gepzrlwzz.sHtML

[S50] C++：格式化数字
来源：http://mobile.sjlbkw.cn/Article/details/gmfkfohgd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gikhhmtle.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fktsv.cn/Article/details/gwkymbivq.sHtML

static_cast<double>(a) / b
来源：http://3g.fktsv.cn/Article/details/gtsawocin.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.bbcook.cn/Article/details/gxanqonia.sHtML

int size() const noexcept { return n_; }
来源：http://blog.bbcook.cn/Article/details/gyobklllz.sHtML

[S53] C++：移动语义
来源：http://mobile.tarul.cn/Article/details/gooyzyume.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.vehdjk.com/Article/details/gytjyirnn.sHtML

[S54] C++：异常处理
来源：http://baike.yfazqb.com/Article/details/gdnmicmmt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.yfazqb.com/Article/details/gicfwlyen.sHtML

[S55] C++：结构化绑定
来源：http://blog.sjlbkw.cn/Article/details/gdatiwpsy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.bbcook.cn/Article/details/gfenukkqr.sHtML

[S56] C++：optional
来源：http://www.share.bbcook.cn/Article/details/gvllfcjkc.sHtML


<!-- 参考信息 -->