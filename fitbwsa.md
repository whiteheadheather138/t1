代发 wailian999

[Q82] 字符长度与字节长度
来源：http://3g.vehdjk.com/Article/details/glnhuxwqc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gnqthhdjd.sHtML

[Q83] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gnyriwgvy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/guhejbhdh.sHtML

[Q84] 去除首尾空格
来源：http://blog.bbcook.cn/Article/details/ghonnqtha.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gansiysnj.sHtML

[Q85] 数值取整
来源：http://baike.bbcook.cn/Article/details/gsrxlwbao.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fktsv.cn/Article/details/gthofmdhq.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.sjlbkw.cn/Article/details/giksshzjy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.yfazqb.com/Article/details/gatbrokij.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fktsv.cn/Article/details/gbqmandph.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.yfazqb.com/Article/details/gewkonlmx.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fktsv.cn/Article/details/glnflkuqu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.yfazqb.com/Article/details/gfvevqfcg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.epnwcf.com/Article/details/gmdfevdtz.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fktsv.cn/Article/details/gewvehtcr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fktsv.cn/Article/details/gdeefirvb.sHtML

[Q90] 生成序号列
来源：http://www.share.yfazqb.com/Article/details/gvpfdmptk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.epnwcf.com/Article/details/gchxvuzxy.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gptrycofv.sHtML

R. Bash 专题
来源：http://baike.sjlbkw.cn/Article/details/ghtzlinuk.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gpunrmlgi.sHtML

[R01] shebang 与严格模式
来源：http://baike.sjlbkw.cn/Article/details/grmxobcsw.sHtML

#!/usr/bin/env bash
来源：http://m.share.epnwcf.com/Article/details/gkblejtix.sHtML

set -euo pipefail
来源：http://m.share.sjlbkw.cn/Article/details/glalffmjy.sHtML

[R02] 变量赋值与使用
来源：http://mobile.bbcook.cn/Article/details/gzysvjbab.sHtML

name="Tom"; echo "$name"
来源：http://wap.fktsv.cn/Article/details/gdxnefnye.sHtML

[R03] 只读变量
来源：http://read.share.vehdjk.com/Article/details/ghzmxkeej.sHtML

readonly PI=3.14
来源：http://www.blog.bbcook.cn/Article/details/gqipsyzqr.sHtML

[R04] 位置参数
来源：http://blog.bbcook.cn/Article/details/gcjkxiikq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fktsv.cn/Article/details/gaeksxhwp.sHtML

[R05] 参数默认值
来源：http://mobile.fktsv.cn/Article/details/gzvbplemr.sHtML

name="${1:-default}"
来源：http://mobile.sjlbkw.cn/Article/details/gybvjsdvd.sHtML

[R06] 判断命令是否存在
来源：http://3g.epnwcf.com/Article/details/gtylapcty.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.tarul.cn/Article/details/glscrerqi.sHtML

[R07] if 判断文件
来源：http://baike.tarul.cn/Article/details/gjbispfjz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.yfazqb.com/Article/details/gootjqkks.sHtML

[R08] 数值比较
来源：http://www.blog.yfazqb.com/Article/details/gkrohzrbh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.sjlbkw.cn/Article/details/gkxaoukow.sHtML

[R09] 字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gyzljbumf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.sjlbkw.cn/Article/details/giwlzqdpe.sHtML

[R10] 正则匹配
来源：http://blog.vehdjk.com/Article/details/govywzryq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.tarul.cn/Article/details/glntdiftm.sHtML

[R11] case 多分支
来源：http://mobile.sjlbkw.cn/Article/details/gdognpiwe.sHtML

case "$1" in
来源：http://m.share.sjlbkw.cn/Article/details/gppquxuxg.sHtML

start) echo "启动" ;;
来源：http://www.share.fktsv.cn/Article/details/grocolzbt.sHtML

stop)  echo "停止" ;;
来源：http://3g.tarul.cn/Article/details/gqmqpctwz.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.vehdjk.com/Article/details/gqspbnhav.sHtML

esac
来源：http://mobile.yfazqb.com/Article/details/gdeccscyr.sHtML

[R12] for 遍历文件
来源：http://mobile.vehdjk.com/Article/details/ghtgsgpgt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fktsv.cn/Article/details/gpstigonx.sHtML

[R13] for 计数循环
来源：http://www.m.share.fktsv.cn/Article/details/gihazcwyl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.vehdjk.com/Article/details/gvxefexcp.sHtML

[R14] C 风格 for
来源：http://www.blog.sjlbkw.cn/Article/details/godsqzzxd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.vehdjk.com/Article/details/gmrwunwea.sHtML

[R15] while 逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gycvjflly.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fktsv.cn/Article/details/gugqzvorx.sHtML

[R16] until 等待条件
来源：http://blog.fktsv.cn/Article/details/gmsfiyukw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/gjrxyapgf.sHtML

[R17] 数组定义与取值
来源：http://read.share.yfazqb.com/Article/details/ghgvfrerb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.tarul.cn/Article/details/gehubknmq.sHtML

[R18] 遍历数组
来源：http://3g.vehdjk.com/Article/details/gwfctrdiq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.vehdjk.com/Article/details/gvlfqyuit.sHtML

[R19] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/gbjyzjmgz.sHtML

echo "${#arr[@]}"
来源：http://read.share.tarul.cn/Article/details/gcmcwccjq.sHtML

[R20] 关联数组（字典）
来源：http://m.share.epnwcf.com/Article/details/gfgkvxywm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.epnwcf.com/Article/details/gxchrjtqx.sHtML

[R21] 字符串长度
来源：http://mobile.yfazqb.com/Article/details/gfmbuewmx.sHtML

echo "${#s}"
来源：http://wap.sjlbkw.cn/Article/details/gtfyfocwm.sHtML

[R22] 截取子串
来源：http://www.m.share.yfazqb.com/Article/details/gnffylgyt.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fktsv.cn/Article/details/gcfvvxnue.sHtML

[R23] 字符串替换
来源：http://www.m.share.vehdjk.com/Article/details/gebfjeydx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.vehdjk.com/Article/details/gdahtidom.sHtML

[R24] 大小写转换
来源：http://3g.epnwcf.com/Article/details/gvbdydptd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.vehdjk.com/Article/details/gyqfuqkgf.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.sjlbkw.cn/Article/details/ggnhydswb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fktsv.cn/Article/details/gcpuxraxy.sHtML

[R26] 命令替换
来源：http://3g.yfazqb.com/Article/details/gwasfkobq.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.yfazqb.com/Article/details/gjkqlxaer.sHtML

[R27] 算术展开
来源：http://3g.bbcook.cn/Article/details/gxuqdaqjj.sHtML

echo $((1 + 2 * 3))
来源：http://blog.tarul.cn/Article/details/gtzhzuwmd.sHtML

[R28] 浮点运算
来源：http://3g.epnwcf.com/Article/details/gmkeviycm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.epnwcf.com/Article/details/gzndauhlt.sHtML

[R29] 定义函数
来源：http://m.share.fktsv.cn/Article/details/gtymfjaah.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.bbcook.cn/Article/details/gwwkwhqma.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.epnwcf.com/Article/details/gsmezgeew.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fktsv.cn/Article/details/grfkmpuex.sHtML

[R31] 局部变量
来源：http://www.share.sjlbkw.cn/Article/details/gqrtozora.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fktsv.cn/Article/details/gyjhatdrd.sHtML

[R32] 参数个数校验
来源：http://m.share.epnwcf.com/Article/details/gknfworwl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gxvqceyoq.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.yfazqb.com/Article/details/gmebnpfoi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fktsv.cn/Article/details/gwfyczcyf.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/gwvvigtsb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/gwntdjurr.sHtML

[R35] 后台执行并等待
来源：http://m.share.sjlbkw.cn/Article/details/geqdtbgjd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.tarul.cn/Article/details/gamjzvqbn.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fktsv.cn/Article/details/ghciuwgfl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fktsv.cn/Article/details/gzjzldrez.sHtML

[R37] 把输出赋给变量
来源：http://blog.vehdjk.com/Article/details/gcmgwdmud.sHtML

files=$(ls -1)
来源：http://www.m.share.yfazqb.com/Article/details/ggdowbzgp.sHtML

[R38] 管道串联
来源：http://wap.fktsv.cn/Article/details/glnfjcfkj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fktsv.cn/Article/details/gnvvcqsot.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fktsv.cn/Article/details/ggslmzgey.sHtML

cmd > out.log 2>&1
来源：http://www.share.tarul.cn/Article/details/gkxsggaml.sHtML

[R40] 追加写日志
来源：http://m.share.yfazqb.com/Article/details/girtduqkj.sHtML

echo "log" >> out.log
来源：http://m.share.yfazqb.com/Article/details/gbctkbybz.sHtML

[R41] 丢弃输出
来源：http://blog.bbcook.cn/Article/details/gwtfdolbz.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.tarul.cn/Article/details/grzgcxdlx.sHtML

[R42] 输入重定向
来源：http://3g.epnwcf.com/Article/details/gzfzktfxl.sHtML

wc -l < a.txt
来源：http://m.share.bbcook.cn/Article/details/gczaobrmt.sHtML

[R43] 按名字查找文件
来源：http://wap.yfazqb.com/Article/details/gcqohzzrn.sHtML

find . -name "*.log" -type f
来源：http://wap.yfazqb.com/Article/details/geuivgrlz.sHtML

[R44] 按修改时间查找
来源：http://mobile.fktsv.cn/Article/details/gajspxtkf.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.epnwcf.com/Article/details/gdtnnsoue.sHtML

[R45] 批量删除
来源：http://mobile.epnwcf.com/Article/details/gslqcjocv.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.vehdjk.com/Article/details/gwxxnqwvz.sHtML

[R46] 递归替换文件内容
来源：http://3g.bbcook.cn/Article/details/gwvsjliir.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.bbcook.cn/Article/details/ghfadsuxo.sHtML

[R47] sed 单行替换
来源：http://www.share.bbcook.cn/Article/details/guujnbiez.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gshuvjgaz.sHtML

[R48] awk 取指定列
来源：http://m.share.bbcook.cn/Article/details/gejnjxgxj.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.tarul.cn/Article/details/grafnlwhu.sHtML

[R49] awk 带条件
来源：http://wap.sjlbkw.cn/Article/details/gknjpuqya.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.bbcook.cn/Article/details/gqdkjzurg.sHtML

[R50] awk 求和
来源：http://www.share.fktsv.cn/Article/details/gstxuowwn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.bbcook.cn/Article/details/gaxqwphpj.sHtML

[R51] 排序去重取前几
来源：http://www.share.yfazqb.com/Article/details/gtdznrsfb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fktsv.cn/Article/details/ghlsyeryd.sHtML

[R52] 统计行数
来源：http://3g.vehdjk.com/Article/details/gtgpyzbsd.sHtML

wc -l a.txt
来源：http://blog.bbcook.cn/Article/details/guvwfytym.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.vehdjk.com/Article/details/glanrlgld.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.bbcook.cn/Article/details/gxzrejjiu.sHtML

[R54] 比较两个文件
来源：http://wap.epnwcf.com/Article/details/ghvrtuzkk.sHtML

diff a.txt b.txt
来源：http://wap.tarul.cn/Article/details/gfmbesujw.sHtML

[R55] 压缩与解压
来源：http://www.m.share.bbcook.cn/Article/details/gpmahxnyn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.vehdjk.com/Article/details/gxxrwgdyt.sHtML

[R56] 远程拷贝
来源：http://baike.sjlbkw.cn/Article/details/gtqdhpkzz.sHtML

scp file user@host:/path/
来源：http://wap.yfazqb.com/Article/details/giknlrwyp.sHtML

[R57] 远程执行命令
来源：http://m.share.yfazqb.com/Article/details/gzxtzriyd.sHtML

ssh user@host 'uptime'
来源：http://www.blog.vehdjk.com/Article/details/gggcdidxi.sHtML

[R58] 下载文件
来源：http://baike.epnwcf.com/Article/details/gcoqicwjg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.tarul.cn/Article/details/gtdenbajc.sHtML

[R59] 发 POST JSON
来源：http://mobile.vehdjk.com/Article/details/gnpcyvztb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.tarul.cn/Article/details/gnapcjkdo.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.tarul.cn/Article/details/gkavzblpb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.bbcook.cn/Article/details/gkjfvrcgr.sHtML

[R61] 磁盘占用
来源：http://blog.fktsv.cn/Article/details/gdusaeyvp.sHtML

df -h;  du -sh *
来源：http://3g.fktsv.cn/Article/details/gincplbjh.sHtML

[R62] 找最占空间的文件
来源：http://3g.vehdjk.com/Article/details/gxynatscm.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fktsv.cn/Article/details/gvfnhemax.sHtML

[R63] 内存与进程
来源：http://m.share.vehdjk.com/Article/details/giusovbjy.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.epnwcf.com/Article/details/gafqiwpxl.sHtML

[R64] 结束进程
来源：http://www.share.fktsv.cn/Article/details/ghlbvfsol.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.tarul.cn/Article/details/ggqwqpyhr.sHtML

[R65] 查看端口占用
来源：http://wap.sjlbkw.cn/Article/details/gpyibmaac.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.bbcook.cn/Article/details/gahzoizvy.sHtML

[R66] 定时任务
来源：http://www.blog.vehdjk.com/Article/details/gdsmybami.sHtML

crontab -e;  crontab -l
来源：http://mobile.bbcook.cn/Article/details/gyfpbycur.sHtML

[R67] 生成随机十六进制串
来源：http://3g.bbcook.cn/Article/details/gyhctreps.sHtML

openssl rand -hex 16
来源：http://mobile.bbcook.cn/Article/details/ghpexttss.sHtML

[R68] 计算文件校验值
来源：http://read.share.tarul.cn/Article/details/gddiwjfdm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.tarul.cn/Article/details/greznlxxv.sHtML

[R69] 生成随机密码
来源：http://3g.yfazqb.com/Article/details/gqsyhhofu.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.yfazqb.com/Article/details/gipiisbsy.sHtML

[R70] 时间戳与互转
来源：http://m.share.epnwcf.com/Article/details/guddlyupk.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.yfazqb.com/Article/details/gfuwtxuup.sHtML

[R71] 日期格式化
来源：http://blog.fktsv.cn/Article/details/gkwaxrqow.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.yfazqb.com/Article/details/gvqsjhkju.sHtML

[R72] 等待端口就绪
来源：http://mobile.bbcook.cn/Article/details/guuepconu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/gbgtlzwue.sHtML

[R73] 分割大日志
来源：http://3g.sjlbkw.cn/Article/details/gpexrqfmh.sHtML

split -l 1000 big.log part_
来源：http://baike.fktsv.cn/Article/details/geqcwazac.sHtML

[R74] 批量重命名
来源：http://baike.epnwcf.com/Article/details/gzgaildtv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.tarul.cn/Article/details/gjxboyhte.sHtML

[R75] 导出环境变量
来源：http://blog.fktsv.cn/Article/details/gmnuhmdzt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.epnwcf.com/Article/details/gxjltavod.sHtML

[R76] 使用临时文件
来源：http://read.share.fktsv.cn/Article/details/gmuqsrqgv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.yfazqb.com/Article/details/gdyitszjj.sHtML

[R77] 读取用户输入
来源：http://www.blog.fktsv.cn/Article/details/ggizokjvo.sHtML

read -rp "请输入: " ans
来源：http://3g.fktsv.cn/Article/details/gbtjttnxn.sHtML

[R78] 交互式菜单
来源：http://3g.yfazqb.com/Article/details/gprxzhrhn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.yfazqb.com/Article/details/gfucedokc.sHtML

[R79] 解析命令行选项
来源：http://3g.sjlbkw.cn/Article/details/gfcvzfgxr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fktsv.cn/Article/details/gxjdjsmud.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.vehdjk.com/Article/details/gxvcyzxby.sHtML

time ./run.sh
来源：http://mobile.sjlbkw.cn/Article/details/gtaxutjxj.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gjjqbxxym.sHtML

S. C / C++ 专题
来源：http://read.share.sjlbkw.cn/Article/details/gsmldekug.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gzlulgmxh.sHtML

[S01] C：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gfqgjrqsr.sHtML

#include <stdio.h>
来源：http://wap.vehdjk.com/Article/details/gznlfvxft.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fktsv.cn/Article/details/gucvadezn.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fktsv.cn/Article/details/gcqbrgtls.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.sjlbkw.cn/Article/details/gzdtfacao.sHtML

[S03] C：读入整数
来源：http://blog.tarul.cn/Article/details/gybztuguz.sHtML

int x; scanf("%d", &x);
来源：http://m.share.epnwcf.com/Article/details/gcjsxbfyf.sHtML

[S04] C：字符串复制
来源：http://blog.yfazqb.com/Article/details/grshnmnje.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.vehdjk.com/Article/details/gsxubbmuj.sHtML

[S05] C：字符串长度
来源：http://blog.bbcook.cn/Article/details/gudptzdhg.sHtML

strlen(s)
来源：http://m.share.yfazqb.com/Article/details/grdnklzie.sHtML

[S06] C：字符串比较
来源：http://www.share.epnwcf.com/Article/details/gniuppovv.sHtML

strcmp(a, b) == 0
来源：http://m.share.vehdjk.com/Article/details/gyglmseab.sHtML

[S07] C：数组遍历求和
来源：http://m.share.sjlbkw.cn/Article/details/gbiewtqge.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.bbcook.cn/Article/details/gswhnjtaz.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.epnwcf.com/Article/details/gnjpqcsoa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fktsv.cn/Article/details/gxtxbsbtw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fktsv.cn/Article/details/gznysygik.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fktsv.cn/Article/details/gtynsvtre.sHtML

[S10] C：指针与解引用
来源：http://3g.bbcook.cn/Article/details/gvjusxoqp.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fktsv.cn/Article/details/ggnymtlgq.sHtML

[S11] C：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gulrhnjwx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.yfazqb.com/Article/details/gulmkbncu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.bbcook.cn/Article/details/gxuukjxwu.sHtML

fclose(f);
来源：http://m.share.yfazqb.com/Article/details/ghpavzdcx.sHtML

[S12] C：写文件
来源：http://m.share.tarul.cn/Article/details/grxqmvuls.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gjivgevbs.sHtML

[S13] C：宏定义
来源：http://www.share.sjlbkw.cn/Article/details/gipbqedyv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.bbcook.cn/Article/details/gyngkyuwr.sHtML

[S14] C：枚举
来源：http://www.share.yfazqb.com/Article/details/gerlspqfz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.tarul.cn/Article/details/gkcykueyx.sHtML

[S15] C：类型转换
来源：http://www.blog.tarul.cn/Article/details/gisqznmex.sHtML

(double) a / b
来源：http://m.share.tarul.cn/Article/details/gsqjiupvq.sHtML

[S16] C：位操作置位
来源：http://3g.fktsv.cn/Article/details/gjtfmgdpb.sHtML

x |= (1 << 3);
来源：http://3g.fktsv.cn/Article/details/gkildozbg.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.vehdjk.com/Article/details/goewpuclh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fktsv.cn/Article/details/ghnloeinw.sHtML

[S18] C：命令行参数
来源：http://m.share.tarul.cn/Article/details/gjxqcycfu.sHtML

int main(int argc, char **argv)
来源：http://3g.vehdjk.com/Article/details/gnkidudny.sHtML

[S19] C：快速排序
来源：http://www.m.share.tarul.cn/Article/details/ggidxhksq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gkuqckcke.sHtML

[S20] C：二分查找
来源：http://www.m.share.yfazqb.com/Article/details/gnludksuu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/gzmfkaywh.sHtML

[S21] C：字符类别判断
来源：http://3g.fktsv.cn/Article/details/glzkabocq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.epnwcf.com/Article/details/ggfzjkiau.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fktsv.cn/Article/details/gsblsvizi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.bbcook.cn/Article/details/gqygcevff.sHtML

[S23] C：随机数
来源：http://m.share.yfazqb.com/Article/details/grzitwtzv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.bbcook.cn/Article/details/gbgiisnvd.sHtML

[S24] C：获取本地时间
来源：http://blog.fktsv.cn/Article/details/gdsiylmgi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.sjlbkw.cn/Article/details/gydpggipz.sHtML

[S25] C：内存拷贝
来源：http://m.share.bbcook.cn/Article/details/gnymvjsdi.sHtML

memcpy(dst, src, n);
来源：http://wap.bbcook.cn/Article/details/ghcluznwp.sHtML

[S26] C：内存清零
来源：http://www.share.fktsv.cn/Article/details/gdyhjatci.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.tarul.cn/Article/details/ggvzclmsm.sHtML

[S27] C：定义常量
来源：http://read.share.epnwcf.com/Article/details/gsshvewmb.sHtML

const double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gcirwhmht.sHtML

[S28] C：静态变量
来源：http://wap.bbcook.cn/Article/details/gaoretpqr.sHtML

static int counter = 0;
来源：http://3g.yfazqb.com/Article/details/gupqmbodl.sHtML

[S29] C：变参函数
来源：http://m.share.epnwcf.com/Article/details/gmxjfbfuc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.yfazqb.com/Article/details/gnmrrkvcr.sHtML

[S30] C：头文件保护
来源：http://blog.yfazqb.com/Article/details/gkojxqtve.sHtML

#ifndef X_H
来源：http://mobile.yfazqb.com/Article/details/grixdymlz.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/graujlzir.sHtML

#endif
来源：http://www.m.share.fktsv.cn/Article/details/gzhfbcjhi.sHtML

[S31] C++：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gvnjlmtxy.sHtML

#include <iostream>
来源：http://wap.tarul.cn/Article/details/ggiaxzvli.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.bbcook.cn/Article/details/gnmasuntp.sHtML

[S32] C++：字符串
来源：http://m.share.epnwcf.com/Article/details/gborfoioh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.tarul.cn/Article/details/ghwtonvws.sHtML

[S33] C++：vector 增删
来源：http://baike.vehdjk.com/Article/details/gzwiuljhn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.yfazqb.com/Article/details/gfeyaoame.sHtML

[S34] C++：遍历 vector
来源：http://mobile.tarul.cn/Article/details/gcbxovshs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.yfazqb.com/Article/details/gnlucbjja.sHtML

[S35] C++：map
来源：http://www.share.bbcook.cn/Article/details/gpfxxkrhv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gvwmtavih.sHtML

[S36] C++：unordered_map
来源：http://read.share.yfazqb.com/Article/details/ghqbqkoxm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gqefmuwqj.sHtML

[S37] C++：set
来源：http://wap.epnwcf.com/Article/details/gicmsjrjn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.tarul.cn/Article/details/gntaansqx.sHtML

[S38] C++：排序
来源：http://3g.fktsv.cn/Article/details/gytylnzwl.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.epnwcf.com/Article/details/gzkgfryoa.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.epnwcf.com/Article/details/gueteouww.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.tarul.cn/Article/details/gfvprdrds.sHtML

[S40] C++：查找元素
来源：http://blog.sjlbkw.cn/Article/details/gtjrsvyah.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.bbcook.cn/Article/details/gwpizltdq.sHtML

[S41] C++：类与构造函数
来源：http://blog.bbcook.cn/Article/details/gceztxvgs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.yfazqb.com/Article/details/gwzaulyel.sHtML

[S42] C++：继承与虚函数
来源：http://blog.tarul.cn/Article/details/gsmixgdnp.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.sjlbkw.cn/Article/details/gdsjyagcb.sHtML

[S43] C++：智能指针
来源：http://m.share.epnwcf.com/Article/details/gswuhmsij.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fktsv.cn/Article/details/gzxtsvlew.sHtML

[S44] C++：引用传参
来源：http://wap.vehdjk.com/Article/details/guayjgvsp.sHtML

void inc(int &x) { ++x; }
来源：http://baike.bbcook.cn/Article/details/gkjhxraqa.sHtML

[S45] C++：lambda
来源：http://3g.tarul.cn/Article/details/guvsityqa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.sjlbkw.cn/Article/details/gcztmteht.sHtML

[S46] C++：函数模板
来源：http://m.share.epnwcf.com/Article/details/ghpmgqwjs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fktsv.cn/Article/details/gsrmculgz.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.epnwcf.com/Article/details/gonytmjgj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.yfazqb.com/Article/details/gllezxrlg.sHtML

[S48] C++：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gejtceqqd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.yfazqb.com/Article/details/gbmsweveo.sHtML

while (std::getline(in, line)) { }
来源：http://baike.vehdjk.com/Article/details/gqgtlvstn.sHtML

[S49] C++：写文件
来源：http://mobile.fktsv.cn/Article/details/goqjcbkbp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fktsv.cn/Article/details/ghwtnixva.sHtML

[S50] C++：格式化数字
来源：http://read.share.yfazqb.com/Article/details/ghtqjkvxf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gmgxrfbyi.sHtML

[S51] C++：显式类型转换
来源：http://baike.tarul.cn/Article/details/gvfbatsev.sHtML

static_cast<double>(a) / b
来源：http://www.share.vehdjk.com/Article/details/guuqrhhid.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.sjlbkw.cn/Article/details/glklbwdei.sHtML


<!-- 参考信息 -->