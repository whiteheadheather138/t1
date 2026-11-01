代发 wailian999

[Q84] 去除首尾空格
来源：http://www.blog.sjlbkw.cn/Article/details/gnruztkdu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gvjdsasds.sHtML

[Q85] 数值取整
来源：http://wap.sjlbkw.cn/Article/details/guxigplrk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.sjlbkw.cn/Article/details/grydqkgiw.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.tarul.cn/Article/details/ghvezkmyq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fktsv.cn/Article/details/gsrjykxoc.sHtML

[Q87] JSON 字段做条件
来源：http://3g.epnwcf.com/Article/details/gdfzxdoba.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.yfazqb.com/Article/details/gbpuezmpl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.tarul.cn/Article/details/gyjmlspqf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.tarul.cn/Article/details/gbcxxyozv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/guqmqiiwu.sHtML

[Q89] 判断表是否存在
来源：http://baike.bbcook.cn/Article/details/gislcigad.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.sjlbkw.cn/Article/details/gxfrbsfez.sHtML

[Q90] 生成序号列
来源：http://www.share.sjlbkw.cn/Article/details/gejiftncq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fktsv.cn/Article/details/grgxksgqf.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gywvppxwz.sHtML

R. Bash 专题
来源：http://3g.vehdjk.com/Article/details/geibujcix.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gkgkulcem.sHtML

[R01] shebang 与严格模式
来源：http://mobile.epnwcf.com/Article/details/gznggwyie.sHtML

#!/usr/bin/env bash
来源：http://www.share.vehdjk.com/Article/details/gqwgkuasp.sHtML

set -euo pipefail
来源：http://3g.epnwcf.com/Article/details/gycqitjjf.sHtML

[R02] 变量赋值与使用
来源：http://blog.fktsv.cn/Article/details/gpzqvwiwg.sHtML

name="Tom"; echo "$name"
来源：http://wap.sjlbkw.cn/Article/details/gfrmuotzu.sHtML

[R03] 只读变量
来源：http://3g.yfazqb.com/Article/details/ghwtqzunh.sHtML

readonly PI=3.14
来源：http://blog.yfazqb.com/Article/details/gbydbpxvm.sHtML

[R04] 位置参数
来源：http://blog.sjlbkw.cn/Article/details/guzxepfkk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.vehdjk.com/Article/details/gmfkbigcz.sHtML

[R05] 参数默认值
来源：http://read.share.sjlbkw.cn/Article/details/gwkywggsf.sHtML

name="${1:-default}"
来源：http://blog.sjlbkw.cn/Article/details/gjwurjiql.sHtML

[R06] 判断命令是否存在
来源：http://blog.tarul.cn/Article/details/glhoqmjzy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.sjlbkw.cn/Article/details/gacptlstx.sHtML

[R07] if 判断文件
来源：http://3g.tarul.cn/Article/details/gxsplhmbu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.epnwcf.com/Article/details/ghxvdezan.sHtML

[R08] 数值比较
来源：http://m.share.tarul.cn/Article/details/gnxrjbqhn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fktsv.cn/Article/details/gkfjmhmno.sHtML

[R09] 字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gwrvznnju.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.bbcook.cn/Article/details/gakcvappx.sHtML

[R10] 正则匹配
来源：http://m.share.epnwcf.com/Article/details/gpmqzltbl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fktsv.cn/Article/details/gvamzqskj.sHtML

[R11] case 多分支
来源：http://www.blog.tarul.cn/Article/details/gfmddllwc.sHtML

case "$1" in
来源：http://3g.sjlbkw.cn/Article/details/gecrpxqcw.sHtML

start) echo "启动" ;;
来源：http://www.blog.epnwcf.com/Article/details/gmtionqnc.sHtML

stop)  echo "停止" ;;
来源：http://m.share.epnwcf.com/Article/details/gtgxdbsxx.sHtML

*)     echo "未知命令" ;;
来源：http://blog.yfazqb.com/Article/details/gszxsunbm.sHtML

esac
来源：http://www.m.share.vehdjk.com/Article/details/gdriwszto.sHtML

[R12] for 遍历文件
来源：http://wap.sjlbkw.cn/Article/details/gtpvuhnla.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.epnwcf.com/Article/details/gdupkxdlj.sHtML

[R13] for 计数循环
来源：http://www.blog.bbcook.cn/Article/details/gqgyjoggy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/gmgokvoiu.sHtML

[R14] C 风格 for
来源：http://3g.sjlbkw.cn/Article/details/gmuokjzri.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.yfazqb.com/Article/details/gjotqvqkz.sHtML

[R15] while 逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gxpavqdmt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.bbcook.cn/Article/details/gicbjaren.sHtML

[R16] until 等待条件
来源：http://mobile.tarul.cn/Article/details/gbpappyjz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/ghcdnylzq.sHtML

[R17] 数组定义与取值
来源：http://m.share.vehdjk.com/Article/details/gxlqdbyht.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.epnwcf.com/Article/details/gakdqevfa.sHtML

[R18] 遍历数组
来源：http://wap.fktsv.cn/Article/details/gpyxprbbo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.epnwcf.com/Article/details/gznveargd.sHtML

[R19] 数组长度
来源：http://baike.epnwcf.com/Article/details/gvrwnnngo.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.tarul.cn/Article/details/grhsicouw.sHtML

[R20] 关联数组（字典）
来源：http://read.share.yfazqb.com/Article/details/gqgvvmmly.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.yfazqb.com/Article/details/gorlscvlr.sHtML

[R21] 字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gljrbtjld.sHtML

echo "${#s}"
来源：http://mobile.epnwcf.com/Article/details/gjardgvac.sHtML

[R22] 截取子串
来源：http://m.share.tarul.cn/Article/details/gceupwznb.sHtML

echo "${s:0:5}"
来源：http://www.blog.yfazqb.com/Article/details/gbmdywzjz.sHtML

[R23] 字符串替换
来源：http://3g.tarul.cn/Article/details/gbluqjwml.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.epnwcf.com/Article/details/ggzzmudrw.sHtML

[R24] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gdyexriou.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.yfazqb.com/Article/details/gdcszqqpb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.bbcook.cn/Article/details/gbjyfnbdc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.bbcook.cn/Article/details/gixuuazre.sHtML

[R26] 命令替换
来源：http://3g.epnwcf.com/Article/details/glqqorllm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.bbcook.cn/Article/details/gylxozewp.sHtML

[R27] 算术展开
来源：http://m.share.fktsv.cn/Article/details/grnddlqob.sHtML

echo $((1 + 2 * 3))
来源：http://blog.vehdjk.com/Article/details/goxkjotlm.sHtML

[R28] 浮点运算
来源：http://wap.sjlbkw.cn/Article/details/gfalwzwsg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.tarul.cn/Article/details/gngwsdcvt.sHtML

[R29] 定义函数
来源：http://3g.fktsv.cn/Article/details/gyfhhuvjj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.vehdjk.com/Article/details/gvmnhhabo.sHtML

[R30] 函数返回状态码
来源：http://blog.yfazqb.com/Article/details/gbucfhqym.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.yfazqb.com/Article/details/gbdyvlanm.sHtML

[R31] 局部变量
来源：http://www.m.share.vehdjk.com/Article/details/grxtyoddg.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fktsv.cn/Article/details/gvvrmfbqu.sHtML

[R32] 参数个数校验
来源：http://www.m.share.epnwcf.com/Article/details/gvppzkhme.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/gzljukszv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnhdpawk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.sjlbkw.cn/Article/details/gnxyzscbt.sHtML

[R34] 退出时清理
来源：http://read.share.fktsv.cn/Article/details/gfuhkhllh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fktsv.cn/Article/details/gxzrlofpx.sHtML

[R35] 后台执行并等待
来源：http://blog.fktsv.cn/Article/details/gcrzfbzwi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.bbcook.cn/Article/details/gmmxrmwhd.sHtML

[R36] 并发执行多个任务
来源：http://blog.vehdjk.com/Article/details/gaosojmqc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.vehdjk.com/Article/details/gxolbqnss.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.bbcook.cn/Article/details/gxhjnmjfa.sHtML

files=$(ls -1)
来源：http://baike.tarul.cn/Article/details/gqadamxyp.sHtML

[R38] 管道串联
来源：http://baike.epnwcf.com/Article/details/givxapbhk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.epnwcf.com/Article/details/gmlbtlcey.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.yfazqb.com/Article/details/glthnagtz.sHtML

cmd > out.log 2>&1
来源：http://3g.vehdjk.com/Article/details/gyklcraky.sHtML

[R40] 追加写日志
来源：http://m.share.sjlbkw.cn/Article/details/gxprlzizp.sHtML

echo "log" >> out.log
来源：http://www.blog.bbcook.cn/Article/details/gxkfdmhla.sHtML

[R41] 丢弃输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gzepjnvhx.sHtML

cmd >/dev/null 2>&1
来源：http://baike.vehdjk.com/Article/details/gxrqoucqg.sHtML

[R42] 输入重定向
来源：http://m.share.yfazqb.com/Article/details/guhntxwez.sHtML

wc -l < a.txt
来源：http://www.share.vehdjk.com/Article/details/gbycozepm.sHtML

[R43] 按名字查找文件
来源：http://www.blog.epnwcf.com/Article/details/gzxjpqnsj.sHtML

find . -name "*.log" -type f
来源：http://baike.sjlbkw.cn/Article/details/gkxyrakbv.sHtML

[R44] 按修改时间查找
来源：http://www.share.epnwcf.com/Article/details/gjdyubzdy.sHtML

find . -mtime -7 -type f
来源：http://3g.bbcook.cn/Article/details/gxcxxtegx.sHtML

[R45] 批量删除
来源：http://www.blog.bbcook.cn/Article/details/gqyogpovq.sHtML

find . -name "*.tmp" -delete
来源：http://baike.sjlbkw.cn/Article/details/gkptukyqi.sHtML

[R46] 递归替换文件内容
来源：http://mobile.epnwcf.com/Article/details/govhtozkd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fktsv.cn/Article/details/gaamnuxkr.sHtML

[R47] sed 单行替换
来源：http://wap.yfazqb.com/Article/details/gobxnibbf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.bbcook.cn/Article/details/gjpiodpzf.sHtML

[R48] awk 取指定列
来源：http://wap.bbcook.cn/Article/details/gezxvdopo.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.vehdjk.com/Article/details/glrqwjyju.sHtML

[R49] awk 带条件
来源：http://wap.bbcook.cn/Article/details/gcdbsluku.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.yfazqb.com/Article/details/gtcxfodrd.sHtML

[R50] awk 求和
来源：http://www.share.yfazqb.com/Article/details/gvxmwrgoz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.epnwcf.com/Article/details/gqbktnekz.sHtML

[R51] 排序去重取前几
来源：http://3g.bbcook.cn/Article/details/gmqkfmcrv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.vehdjk.com/Article/details/glwxdkvcy.sHtML

[R52] 统计行数
来源：http://m.share.epnwcf.com/Article/details/gltxnsmqi.sHtML

wc -l a.txt
来源：http://mobile.fktsv.cn/Article/details/gzgonratw.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.bbcook.cn/Article/details/gxnbymhwh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.sjlbkw.cn/Article/details/gczjybklq.sHtML

[R54] 比较两个文件
来源：http://baike.bbcook.cn/Article/details/gnilyaqlu.sHtML

diff a.txt b.txt
来源：http://mobile.yfazqb.com/Article/details/gpvymramt.sHtML

[R55] 压缩与解压
来源：http://www.blog.yfazqb.com/Article/details/gwtuhpopi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.vehdjk.com/Article/details/gsgrotvuz.sHtML

[R56] 远程拷贝
来源：http://read.share.yfazqb.com/Article/details/gbqiwtzhs.sHtML

scp file user@host:/path/
来源：http://www.share.vehdjk.com/Article/details/gcucrjows.sHtML

[R57] 远程执行命令
来源：http://baike.tarul.cn/Article/details/gowzkafis.sHtML

ssh user@host 'uptime'
来源：http://mobile.vehdjk.com/Article/details/gzljhjwdx.sHtML

[R58] 下载文件
来源：http://m.share.tarul.cn/Article/details/gljcfkvll.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.bbcook.cn/Article/details/gcxtchkrq.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/gmzvsdiqj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.bbcook.cn/Article/details/gpdfcnigv.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/gaywskzqs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.tarul.cn/Article/details/gkitsdbbw.sHtML

[R61] 磁盘占用
来源：http://www.share.vehdjk.com/Article/details/gbfqcnnxk.sHtML

df -h;  du -sh *
来源：http://wap.yfazqb.com/Article/details/gjzouxfdj.sHtML

[R62] 找最占空间的文件
来源：http://3g.vehdjk.com/Article/details/ggjmqcmph.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.tarul.cn/Article/details/ghnhamndo.sHtML

[R63] 内存与进程
来源：http://m.share.bbcook.cn/Article/details/gcxjtrpcv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.sjlbkw.cn/Article/details/gvjwpihtf.sHtML

[R64] 结束进程
来源：http://www.share.vehdjk.com/Article/details/gdjooggdf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.tarul.cn/Article/details/gssrivjrt.sHtML

[R65] 查看端口占用
来源：http://www.m.share.tarul.cn/Article/details/gvbbvitmz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.tarul.cn/Article/details/glcnjupeo.sHtML

[R66] 定时任务
来源：http://www.m.share.vehdjk.com/Article/details/gyjcirqgv.sHtML

crontab -e;  crontab -l
来源：http://read.share.epnwcf.com/Article/details/gznhuvskm.sHtML

[R67] 生成随机十六进制串
来源：http://baike.vehdjk.com/Article/details/glpzjmmeq.sHtML

openssl rand -hex 16
来源：http://read.share.bbcook.cn/Article/details/gtxfomwan.sHtML

[R68] 计算文件校验值
来源：http://mobile.yfazqb.com/Article/details/girtzqeol.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.tarul.cn/Article/details/gbismqvsb.sHtML

[R69] 生成随机密码
来源：http://blog.vehdjk.com/Article/details/ghdgotyfa.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.epnwcf.com/Article/details/gmgdxvlvl.sHtML

[R70] 时间戳与互转
来源：http://blog.sjlbkw.cn/Article/details/ggwibqokt.sHtML

date +%s;  date -d @1700000000
来源：http://wap.epnwcf.com/Article/details/gznkvxqoz.sHtML

[R71] 日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gturrtrhl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.sjlbkw.cn/Article/details/gotilxeao.sHtML

[R72] 等待端口就绪
来源：http://m.share.fktsv.cn/Article/details/glfvlwrjd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/gqkzxkozn.sHtML

[R73] 分割大日志
来源：http://m.share.bbcook.cn/Article/details/guerzzjhc.sHtML

split -l 1000 big.log part_
来源：http://www.share.tarul.cn/Article/details/grokyeont.sHtML

[R74] 批量重命名
来源：http://wap.epnwcf.com/Article/details/gohzsdvfs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.vehdjk.com/Article/details/gzfqzcemm.sHtML

[R75] 导出环境变量
来源：http://baike.bbcook.cn/Article/details/gsogddhhu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.tarul.cn/Article/details/gkrceaogw.sHtML

[R76] 使用临时文件
来源：http://www.share.sjlbkw.cn/Article/details/ghzonyleg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.sjlbkw.cn/Article/details/gtglxrodj.sHtML

[R77] 读取用户输入
来源：http://3g.bbcook.cn/Article/details/giuupvlae.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.tarul.cn/Article/details/gepvmybab.sHtML

[R78] 交互式菜单
来源：http://www.blog.sjlbkw.cn/Article/details/gpgaznhdv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.tarul.cn/Article/details/ggeztzchg.sHtML

[R79] 解析命令行选项
来源：http://3g.epnwcf.com/Article/details/gjkwwwfsc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.sjlbkw.cn/Article/details/gyvrneivn.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fktsv.cn/Article/details/gcsytifqu.sHtML

time ./run.sh
来源：http://www.blog.sjlbkw.cn/Article/details/gmwrrbpnv.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gxvqvwuyh.sHtML

S. C / C++ 专题
来源：http://3g.bbcook.cn/Article/details/gloakkxro.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gemspqohe.sHtML

[S01] C：Hello World
来源：http://read.share.yfazqb.com/Article/details/ghqqjxejt.sHtML

#include <stdio.h>
来源：http://m.share.bbcook.cn/Article/details/guxhqelag.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.tarul.cn/Article/details/gfjpujbxw.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.epnwcf.com/Article/details/gifxxukaf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.bbcook.cn/Article/details/gvciowsqo.sHtML

[S03] C：读入整数
来源：http://baike.yfazqb.com/Article/details/guuwmmlbi.sHtML

int x; scanf("%d", &x);
来源：http://mobile.vehdjk.com/Article/details/gutaevqgh.sHtML

[S04] C：字符串复制
来源：http://baike.bbcook.cn/Article/details/gqjbotpwk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fktsv.cn/Article/details/gyyiwpefj.sHtML

[S05] C：字符串长度
来源：http://wap.yfazqb.com/Article/details/gipngjgmo.sHtML

strlen(s)
来源：http://mobile.yfazqb.com/Article/details/gplpvudeu.sHtML

[S06] C：字符串比较
来源：http://www.blog.yfazqb.com/Article/details/gpagidtuk.sHtML

strcmp(a, b) == 0
来源：http://m.share.yfazqb.com/Article/details/gmgpzcgdo.sHtML

[S07] C：数组遍历求和
来源：http://wap.bbcook.cn/Article/details/gtbpqewsa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.yfazqb.com/Article/details/gdedzspag.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fktsv.cn/Article/details/gepjoyrvd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fktsv.cn/Article/details/gkjsggvlr.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.tarul.cn/Article/details/gjdsjeljm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.yfazqb.com/Article/details/gxrquweio.sHtML

[S10] C：指针与解引用
来源：http://read.share.sjlbkw.cn/Article/details/ghyffqyvj.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.bbcook.cn/Article/details/gtbnsdhyy.sHtML

[S11] C：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gyahekerr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.tarul.cn/Article/details/gghstynhj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.bbcook.cn/Article/details/gxcijdhyb.sHtML

fclose(f);
来源：http://mobile.yfazqb.com/Article/details/gkjfhcofe.sHtML

[S12] C：写文件
来源：http://blog.vehdjk.com/Article/details/gmmtywota.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gfsqxrhbi.sHtML

[S13] C：宏定义
来源：http://www.blog.bbcook.cn/Article/details/gznpucwyj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.bbcook.cn/Article/details/ghblltqxr.sHtML

[S14] C：枚举
来源：http://read.share.bbcook.cn/Article/details/gwhbeaidr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.sjlbkw.cn/Article/details/glasfkqxc.sHtML

[S15] C：类型转换
来源：http://www.m.share.vehdjk.com/Article/details/gvczmnwbj.sHtML

(double) a / b
来源：http://read.share.vehdjk.com/Article/details/gheutjabb.sHtML

[S16] C：位操作置位
来源：http://mobile.fktsv.cn/Article/details/gbxumonrj.sHtML

x |= (1 << 3);
来源：http://mobile.epnwcf.com/Article/details/goiplbcar.sHtML

[S17] C：安全拼接字符串
来源：http://baike.tarul.cn/Article/details/gilnmssax.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.epnwcf.com/Article/details/gsstzgjws.sHtML

[S18] C：命令行参数
来源：http://www.blog.tarul.cn/Article/details/ggaqrivah.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.vehdjk.com/Article/details/grncgshlv.sHtML

[S19] C：快速排序
来源：http://www.m.share.epnwcf.com/Article/details/ggsnwkceq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.yfazqb.com/Article/details/gcewtketi.sHtML

[S20] C：二分查找
来源：http://3g.vehdjk.com/Article/details/gbwzdvllf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjyrxnkb.sHtML

[S21] C：字符类别判断
来源：http://read.share.tarul.cn/Article/details/gjrrosusc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.sjlbkw.cn/Article/details/geyyqxusc.sHtML

[S22] C：字符串转数字
来源：http://www.share.fktsv.cn/Article/details/gmbbmgyqq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.sjlbkw.cn/Article/details/gylwmqzfk.sHtML

[S23] C：随机数
来源：http://www.blog.epnwcf.com/Article/details/gmfoydzob.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fktsv.cn/Article/details/gwtkgageg.sHtML

[S24] C：获取本地时间
来源：http://blog.tarul.cn/Article/details/gwemihslq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.sjlbkw.cn/Article/details/gwoiacmhy.sHtML

[S25] C：内存拷贝
来源：http://wap.fktsv.cn/Article/details/gmtxufjoa.sHtML

memcpy(dst, src, n);
来源：http://blog.yfazqb.com/Article/details/gincueeru.sHtML

[S26] C：内存清零
来源：http://3g.fktsv.cn/Article/details/ghnaugwde.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.epnwcf.com/Article/details/gguuhdvqz.sHtML

[S27] C：定义常量
来源：http://baike.bbcook.cn/Article/details/gxfcuwtoi.sHtML

const double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/geqjpajny.sHtML

[S28] C：静态变量
来源：http://www.share.fktsv.cn/Article/details/gxzyqhjfd.sHtML

static int counter = 0;
来源：http://www.share.vehdjk.com/Article/details/gjwvoeboo.sHtML

[S29] C：变参函数
来源：http://3g.yfazqb.com/Article/details/gskrvrgvq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.epnwcf.com/Article/details/gmisyknhx.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fktsv.cn/Article/details/gvowcmwtx.sHtML

#ifndef X_H
来源：http://m.share.epnwcf.com/Article/details/ghqhvavgo.sHtML

#define X_H
来源：http://read.share.fktsv.cn/Article/details/gctmsorcf.sHtML

#endif
来源：http://mobile.vehdjk.com/Article/details/gdjlhmazo.sHtML

[S31] C++：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gettnbccz.sHtML

#include <iostream>
来源：http://www.blog.tarul.cn/Article/details/ghpkyksvy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.epnwcf.com/Article/details/ggeakdnen.sHtML

[S32] C++：字符串
来源：http://www.share.tarul.cn/Article/details/gqejlcsom.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.sjlbkw.cn/Article/details/gskyvvdje.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.bbcook.cn/Article/details/gssluiuou.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.vehdjk.com/Article/details/gwntujnjm.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.epnwcf.com/Article/details/gqhpzzdxw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.bbcook.cn/Article/details/glwkgomwh.sHtML

[S35] C++：map
来源：http://mobile.sjlbkw.cn/Article/details/grqiohaao.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gkzhwtnwn.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.bbcook.cn/Article/details/gezwdsehk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gxjqdchbg.sHtML

[S37] C++：set
来源：http://read.share.vehdjk.com/Article/details/ggokizpkj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.epnwcf.com/Article/details/gxiyermfz.sHtML

[S38] C++：排序
来源：http://m.share.epnwcf.com/Article/details/gfrvcogwt.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.epnwcf.com/Article/details/glochjigf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.yfazqb.com/Article/details/ghgurnwik.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfnzbhtf.sHtML

[S40] C++：查找元素
来源：http://read.share.vehdjk.com/Article/details/gakbjtgxg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.vehdjk.com/Article/details/gldjlidwl.sHtML

[S41] C++：类与构造函数
来源：http://wap.fktsv.cn/Article/details/gfucfmmgd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.sjlbkw.cn/Article/details/ggejhisqk.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.epnwcf.com/Article/details/gooseuzna.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.vehdjk.com/Article/details/grkucysim.sHtML

[S43] C++：智能指针
来源：http://m.share.sjlbkw.cn/Article/details/gkbuunaxq.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.yfazqb.com/Article/details/gwlxuoolr.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fktsv.cn/Article/details/glrturiib.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.bbcook.cn/Article/details/gthbzdhvh.sHtML

[S45] C++：lambda
来源：http://wap.bbcook.cn/Article/details/gtfaoyuwi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.bbcook.cn/Article/details/glwkxsrao.sHtML

[S46] C++：函数模板
来源：http://www.m.share.yfazqb.com/Article/details/gmfmylwya.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.yfazqb.com/Article/details/gdtwwjnbz.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.epnwcf.com/Article/details/gcetgrheq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.tarul.cn/Article/details/gnkemongs.sHtML

[S48] C++：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gtwtzeomj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.yfazqb.com/Article/details/gywfpcqyb.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fktsv.cn/Article/details/gsntnplpw.sHtML

[S49] C++：写文件
来源：http://3g.tarul.cn/Article/details/gciddubcb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.tarul.cn/Article/details/ghvlclstd.sHtML

[S50] C++：格式化数字
来源：http://www.share.yfazqb.com/Article/details/ghpsljksv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gmbdvvhjl.sHtML

[S51] C++：显式类型转换
来源：http://blog.yfazqb.com/Article/details/gjzmkpyxw.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuaysken.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.vehdjk.com/Article/details/gugljbayt.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.yfazqb.com/Article/details/gywlxwgke.sHtML

[S53] C++：移动语义
来源：http://www.blog.bbcook.cn/Article/details/gbezboorj.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.bbcook.cn/Article/details/grridqnij.sHtML

[S54] C++：异常处理
来源：http://www.m.share.bbcook.cn/Article/details/gokbjhqpe.sHtML


<!-- 参考信息 -->