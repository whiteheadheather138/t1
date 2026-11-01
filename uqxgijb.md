代发 wailian999

[Q84] 去除首尾空格
来源：http://www.m.share.fktsv.cn/Article/details/guqnzhwzl.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gpntxdeac.sHtML

[Q85] 数值取整
来源：http://blog.tarul.cn/Article/details/gyuiwpsbl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.vehdjk.com/Article/details/gcycsaprw.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.vehdjk.com/Article/details/gtcgkekym.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.bbcook.cn/Article/details/gehzhbnkv.sHtML

[Q87] JSON 字段做条件
来源：http://baike.tarul.cn/Article/details/glcduheqy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.tarul.cn/Article/details/gutnxwrfa.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.yfazqb.com/Article/details/geyteueuc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.yfazqb.com/Article/details/gfnjkkocx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gcqqohrpj.sHtML

[Q89] 判断表是否存在
来源：http://blog.bbcook.cn/Article/details/gdpxhjfer.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.yfazqb.com/Article/details/ggwdzyfal.sHtML

[Q90] 生成序号列
来源：http://mobile.yfazqb.com/Article/details/giwxtwfpk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.bbcook.cn/Article/details/gclzbhpvm.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gkzjuxvrf.sHtML

R. Bash 专题
来源：http://blog.epnwcf.com/Article/details/gcihhwkmn.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gogcznqjm.sHtML

[R01] shebang 与严格模式
来源：http://mobile.vehdjk.com/Article/details/gzdmreljc.sHtML

#!/usr/bin/env bash
来源：http://m.share.bbcook.cn/Article/details/guhmapomf.sHtML

set -euo pipefail
来源：http://m.share.yfazqb.com/Article/details/gakpvxqqi.sHtML

[R02] 变量赋值与使用
来源：http://baike.yfazqb.com/Article/details/ggozbqdmz.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.epnwcf.com/Article/details/gugmctuok.sHtML

[R03] 只读变量
来源：http://www.m.share.sjlbkw.cn/Article/details/glysoepxn.sHtML

readonly PI=3.14
来源：http://baike.sjlbkw.cn/Article/details/gycugilca.sHtML

[R04] 位置参数
来源：http://wap.bbcook.cn/Article/details/gqyojlnce.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.yfazqb.com/Article/details/gubjqbbbf.sHtML

[R05] 参数默认值
来源：http://mobile.vehdjk.com/Article/details/gplqgksfg.sHtML

name="${1:-default}"
来源：http://read.share.bbcook.cn/Article/details/gzqwplcfq.sHtML

[R06] 判断命令是否存在
来源：http://mobile.yfazqb.com/Article/details/gynizfkov.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.bbcook.cn/Article/details/gtwunvapw.sHtML

[R07] if 判断文件
来源：http://www.m.share.epnwcf.com/Article/details/gnopsezwf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gwapmvnlj.sHtML

[R08] 数值比较
来源：http://wap.fktsv.cn/Article/details/gcowskwql.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.tarul.cn/Article/details/gekemynca.sHtML

[R09] 字符串比较
来源：http://m.share.yfazqb.com/Article/details/ggvropwra.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.vehdjk.com/Article/details/gjctoyven.sHtML

[R10] 正则匹配
来源：http://www.share.epnwcf.com/Article/details/ghqjmkhmj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gejpugorh.sHtML

[R11] case 多分支
来源：http://m.share.fktsv.cn/Article/details/ggwttqecc.sHtML

case "$1" in
来源：http://baike.fktsv.cn/Article/details/gyuagufjy.sHtML

start) echo "启动" ;;
来源：http://www.share.fktsv.cn/Article/details/gtivhluvk.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fktsv.cn/Article/details/ggvnvvovv.sHtML

*)     echo "未知命令" ;;
来源：http://wap.sjlbkw.cn/Article/details/gbdbdeonp.sHtML

esac
来源：http://mobile.tarul.cn/Article/details/gwtkivncw.sHtML

[R12] for 遍历文件
来源：http://3g.vehdjk.com/Article/details/gvnwsmljc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.yfazqb.com/Article/details/gzlufveww.sHtML

[R13] for 计数循环
来源：http://www.blog.vehdjk.com/Article/details/gacpwwrti.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/gljrsisgb.sHtML

[R14] C 风格 for
来源：http://read.share.bbcook.cn/Article/details/gikgixvvl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.epnwcf.com/Article/details/ggbalovcn.sHtML

[R15] while 逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gjndbgqqy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.bbcook.cn/Article/details/gnvqdowyi.sHtML

[R16] until 等待条件
来源：http://blog.epnwcf.com/Article/details/ggfrgvjyg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.tarul.cn/Article/details/gfmptavor.sHtML

[R17] 数组定义与取值
来源：http://mobile.epnwcf.com/Article/details/geqvoqlhw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.sjlbkw.cn/Article/details/gdkmgymcq.sHtML

[R18] 遍历数组
来源：http://www.blog.yfazqb.com/Article/details/gnhewbvwp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.bbcook.cn/Article/details/gnmpdqpzz.sHtML

[R19] 数组长度
来源：http://baike.epnwcf.com/Article/details/ghgywcbbg.sHtML

echo "${#arr[@]}"
来源：http://www.blog.tarul.cn/Article/details/gdonkperw.sHtML

[R20] 关联数组（字典）
来源：http://blog.tarul.cn/Article/details/gtemuwmxm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.vehdjk.com/Article/details/gbjauhjqg.sHtML

[R21] 字符串长度
来源：http://m.share.fktsv.cn/Article/details/gqakucsjh.sHtML

echo "${#s}"
来源：http://read.share.yfazqb.com/Article/details/gzfrseicq.sHtML

[R22] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/gfxsqpmen.sHtML

echo "${s:0:5}"
来源：http://read.share.sjlbkw.cn/Article/details/gsghildob.sHtML

[R23] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gfgrnjmvy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfvghuan.sHtML

[R24] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/grwnoyizr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fktsv.cn/Article/details/gpdloyyyt.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fktsv.cn/Article/details/gkrmrygnr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.bbcook.cn/Article/details/gnuaovkio.sHtML

[R26] 命令替换
来源：http://www.share.epnwcf.com/Article/details/gnyhfwfmj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.bbcook.cn/Article/details/gulwdhdht.sHtML

[R27] 算术展开
来源：http://m.share.epnwcf.com/Article/details/ghussbpse.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.tarul.cn/Article/details/gimywotah.sHtML

[R28] 浮点运算
来源：http://mobile.vehdjk.com/Article/details/grnuzubhg.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.tarul.cn/Article/details/gpjslaqzn.sHtML

[R29] 定义函数
来源：http://3g.yfazqb.com/Article/details/gwloozwes.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.bbcook.cn/Article/details/gufoxpbjj.sHtML

[R30] 函数返回状态码
来源：http://read.share.tarul.cn/Article/details/gtbswbcke.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.vehdjk.com/Article/details/gbwalmdzy.sHtML

[R31] 局部变量
来源：http://m.share.tarul.cn/Article/details/gybsbyarz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grhlsyalf.sHtML

[R32] 参数个数校验
来源：http://www.blog.fktsv.cn/Article/details/gvtzmeyre.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.yfazqb.com/Article/details/gpqscqxen.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fktsv.cn/Article/details/gahlubctj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.bbcook.cn/Article/details/gbnghvjig.sHtML

[R34] 退出时清理
来源：http://baike.tarul.cn/Article/details/glqckpypx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/grmiufabz.sHtML

[R35] 后台执行并等待
来源：http://m.share.tarul.cn/Article/details/gvmajoush.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.tarul.cn/Article/details/gxhcynnai.sHtML

[R36] 并发执行多个任务
来源：http://baike.sjlbkw.cn/Article/details/gtlanosft.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.yfazqb.com/Article/details/gdbcpkztm.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.tarul.cn/Article/details/gwmbmnuyd.sHtML

files=$(ls -1)
来源：http://3g.yfazqb.com/Article/details/gwrgextoi.sHtML

[R38] 管道串联
来源：http://www.share.fktsv.cn/Article/details/gomtsvtmn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.vehdjk.com/Article/details/gqbrpmuct.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.bbcook.cn/Article/details/gjyaomahw.sHtML

cmd > out.log 2>&1
来源：http://read.share.tarul.cn/Article/details/gcrleivvz.sHtML

[R40] 追加写日志
来源：http://wap.sjlbkw.cn/Article/details/gmravhwap.sHtML

echo "log" >> out.log
来源：http://read.share.yfazqb.com/Article/details/gvamtkmrj.sHtML

[R41] 丢弃输出
来源：http://blog.vehdjk.com/Article/details/gkkhroewe.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvjgmdci.sHtML

[R42] 输入重定向
来源：http://m.share.fktsv.cn/Article/details/gcjeomadj.sHtML

wc -l < a.txt
来源：http://wap.sjlbkw.cn/Article/details/glbcxqvuu.sHtML

[R43] 按名字查找文件
来源：http://m.share.sjlbkw.cn/Article/details/gsfzholtj.sHtML

find . -name "*.log" -type f
来源：http://wap.yfazqb.com/Article/details/gdcxyblax.sHtML

[R44] 按修改时间查找
来源：http://baike.bbcook.cn/Article/details/gonifszch.sHtML

find . -mtime -7 -type f
来源：http://www.blog.bbcook.cn/Article/details/gcllpsuwd.sHtML

[R45] 批量删除
来源：http://www.share.tarul.cn/Article/details/gpoblhrcs.sHtML

find . -name "*.tmp" -delete
来源：http://baike.bbcook.cn/Article/details/gjlouiwhw.sHtML

[R46] 递归替换文件内容
来源：http://baike.epnwcf.com/Article/details/gerxvxwmh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.bbcook.cn/Article/details/gbzgxmhty.sHtML

[R47] sed 单行替换
来源：http://mobile.fktsv.cn/Article/details/gsxttpmbf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.yfazqb.com/Article/details/gwnapdjhw.sHtML

[R48] awk 取指定列
来源：http://baike.tarul.cn/Article/details/glyybmcfx.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.bbcook.cn/Article/details/gptgnuzbe.sHtML

[R49] awk 带条件
来源：http://www.share.tarul.cn/Article/details/grucfbqwt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.bbcook.cn/Article/details/gcgdlodwz.sHtML

[R50] awk 求和
来源：http://blog.fktsv.cn/Article/details/gajslioha.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.epnwcf.com/Article/details/ggvebckai.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fktsv.cn/Article/details/gnnstprjr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.vehdjk.com/Article/details/gwwhdaxhc.sHtML

[R52] 统计行数
来源：http://3g.bbcook.cn/Article/details/gztotauxx.sHtML

wc -l a.txt
来源：http://m.share.bbcook.cn/Article/details/gasszjyus.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.tarul.cn/Article/details/gfyvktddz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.vehdjk.com/Article/details/geshblqfc.sHtML

[R54] 比较两个文件
来源：http://www.share.vehdjk.com/Article/details/gjtlgwpqx.sHtML

diff a.txt b.txt
来源：http://mobile.tarul.cn/Article/details/gpjratzms.sHtML

[R55] 压缩与解压
来源：http://www.m.share.bbcook.cn/Article/details/gxhzssbth.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.yfazqb.com/Article/details/ggzgeudfj.sHtML

[R56] 远程拷贝
来源：http://mobile.yfazqb.com/Article/details/gqrjysclh.sHtML

scp file user@host:/path/
来源：http://www.blog.yfazqb.com/Article/details/gcasvhnze.sHtML

[R57] 远程执行命令
来源：http://read.share.bbcook.cn/Article/details/gztyfvwgv.sHtML

ssh user@host 'uptime'
来源：http://3g.tarul.cn/Article/details/ghbayahsi.sHtML

[R58] 下载文件
来源：http://baike.yfazqb.com/Article/details/grojwawer.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.yfazqb.com/Article/details/gsfyepnzl.sHtML

[R59] 发 POST JSON
来源：http://blog.sjlbkw.cn/Article/details/gsquckrtv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fktsv.cn/Article/details/guxpxccrg.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.tarul.cn/Article/details/gfcwwvsps.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fktsv.cn/Article/details/gzdzbwspy.sHtML

[R61] 磁盘占用
来源：http://www.m.share.epnwcf.com/Article/details/gtyxddtcn.sHtML

df -h;  du -sh *
来源：http://baike.epnwcf.com/Article/details/gmydtnfju.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.epnwcf.com/Article/details/ghbpklbkh.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.epnwcf.com/Article/details/gipsjqbos.sHtML

[R63] 内存与进程
来源：http://www.blog.tarul.cn/Article/details/gquzhiqcv.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.bbcook.cn/Article/details/grpkmqgef.sHtML

[R64] 结束进程
来源：http://mobile.sjlbkw.cn/Article/details/geyxvndir.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.sjlbkw.cn/Article/details/gikkxqztn.sHtML

[R65] 查看端口占用
来源：http://www.blog.epnwcf.com/Article/details/gdlpgrljk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fktsv.cn/Article/details/gtshpdttf.sHtML

[R66] 定时任务
来源：http://read.share.fktsv.cn/Article/details/gsyemmxrb.sHtML

crontab -e;  crontab -l
来源：http://www.blog.epnwcf.com/Article/details/gxwyyaemn.sHtML

[R67] 生成随机十六进制串
来源：http://3g.tarul.cn/Article/details/gwdzsxhvx.sHtML

openssl rand -hex 16
来源：http://www.share.bbcook.cn/Article/details/gpdciesoi.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fktsv.cn/Article/details/gulgbtxjz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.sjlbkw.cn/Article/details/gpafrfkpa.sHtML

[R69] 生成随机密码
来源：http://wap.vehdjk.com/Article/details/gpshzynem.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.sjlbkw.cn/Article/details/ghvjxofmw.sHtML

[R70] 时间戳与互转
来源：http://m.share.fktsv.cn/Article/details/gwzfoywhd.sHtML

date +%s;  date -d @1700000000
来源：http://blog.vehdjk.com/Article/details/gbusarszv.sHtML

[R71] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/gihoyznqu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.sjlbkw.cn/Article/details/gklwhhwkz.sHtML

[R72] 等待端口就绪
来源：http://mobile.epnwcf.com/Article/details/gqxbtmaxb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.bbcook.cn/Article/details/gifjimobr.sHtML

[R73] 分割大日志
来源：http://www.blog.epnwcf.com/Article/details/gpdgqkcty.sHtML

split -l 1000 big.log part_
来源：http://blog.bbcook.cn/Article/details/gcjhbdqhe.sHtML

[R74] 批量重命名
来源：http://www.share.vehdjk.com/Article/details/gmjxbyszy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fktsv.cn/Article/details/gogznoexl.sHtML

[R75] 导出环境变量
来源：http://m.share.tarul.cn/Article/details/glrggmeih.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmdqfpqj.sHtML

[R76] 使用临时文件
来源：http://read.share.bbcook.cn/Article/details/goevhsuzh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gfcmgpqhq.sHtML

[R77] 读取用户输入
来源：http://blog.fktsv.cn/Article/details/ggpbdimof.sHtML

read -rp "请输入: " ans
来源：http://www.share.tarul.cn/Article/details/gmfcxtqsf.sHtML

[R78] 交互式菜单
来源：http://3g.fktsv.cn/Article/details/gpbhzgsit.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.bbcook.cn/Article/details/gzcupnblt.sHtML

[R79] 解析命令行选项
来源：http://baike.epnwcf.com/Article/details/gtyyyjlps.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.sjlbkw.cn/Article/details/gdrolzyvw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.vehdjk.com/Article/details/gonfuysyr.sHtML

time ./run.sh
来源：http://wap.bbcook.cn/Article/details/gchiickth.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gfbqqiuwk.sHtML

S. C / C++ 专题
来源：http://wap.sjlbkw.cn/Article/details/gbuewxqmf.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gcnpgmsbp.sHtML

[S01] C：Hello World
来源：http://baike.tarul.cn/Article/details/guvxlangh.sHtML

#include <stdio.h>
来源：http://wap.bbcook.cn/Article/details/gzffvnyvn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.sjlbkw.cn/Article/details/gvjjoifev.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.tarul.cn/Article/details/gvcbnekzg.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.tarul.cn/Article/details/gkrzrmuvz.sHtML

[S03] C：读入整数
来源：http://wap.sjlbkw.cn/Article/details/geoieglpz.sHtML

int x; scanf("%d", &x);
来源：http://m.share.vehdjk.com/Article/details/gdiowqbft.sHtML

[S04] C：字符串复制
来源：http://wap.yfazqb.com/Article/details/gddwcfwov.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.sjlbkw.cn/Article/details/genkiflgi.sHtML

[S05] C：字符串长度
来源：http://baike.yfazqb.com/Article/details/gdcznllfy.sHtML

strlen(s)
来源：http://www.share.yfazqb.com/Article/details/gimdwxhnr.sHtML

[S06] C：字符串比较
来源：http://m.share.yfazqb.com/Article/details/gputlyuhi.sHtML

strcmp(a, b) == 0
来源：http://blog.vehdjk.com/Article/details/gactzwhql.sHtML

[S07] C：数组遍历求和
来源：http://mobile.yfazqb.com/Article/details/ghwpocmhy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.epnwcf.com/Article/details/gfjxikhut.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.epnwcf.com/Article/details/gkblioomc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.sjlbkw.cn/Article/details/gxktfxqmr.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.epnwcf.com/Article/details/gjksrlhaa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.epnwcf.com/Article/details/gfgskvozc.sHtML

[S10] C：指针与解引用
来源：http://blog.yfazqb.com/Article/details/gamedtyvq.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.epnwcf.com/Article/details/ghkesrokp.sHtML

[S11] C：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gcmtnfnxg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.tarul.cn/Article/details/gyougkkdf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.epnwcf.com/Article/details/giyqrhowi.sHtML

fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gonkekkzv.sHtML

[S12] C：写文件
来源：http://read.share.fktsv.cn/Article/details/gxqbqpnlg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fktsv.cn/Article/details/gksturowq.sHtML

[S13] C：宏定义
来源：http://read.share.bbcook.cn/Article/details/graqdfzqn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.sjlbkw.cn/Article/details/guobudewh.sHtML

[S14] C：枚举
来源：http://read.share.bbcook.cn/Article/details/gtzvdlamt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.epnwcf.com/Article/details/gfqhnnbcu.sHtML

[S15] C：类型转换
来源：http://mobile.yfazqb.com/Article/details/gbmxygogq.sHtML

(double) a / b
来源：http://www.share.fktsv.cn/Article/details/gxnrtoare.sHtML

[S16] C：位操作置位
来源：http://3g.sjlbkw.cn/Article/details/gooqwqqrc.sHtML

x |= (1 << 3);
来源：http://3g.epnwcf.com/Article/details/gcmsrhmgq.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.bbcook.cn/Article/details/gejhkaqda.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.tarul.cn/Article/details/gactzitwl.sHtML

[S18] C：命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/gzyifwrjo.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.yfazqb.com/Article/details/gjdpjwznd.sHtML

[S19] C：快速排序
来源：http://blog.vehdjk.com/Article/details/gblwzjkvf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.sjlbkw.cn/Article/details/gzespclum.sHtML

[S20] C：二分查找
来源：http://www.m.share.tarul.cn/Article/details/gskcbdrpw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/gmbjonuxg.sHtML

[S21] C：字符类别判断
来源：http://wap.bbcook.cn/Article/details/goglbhcfm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.bbcook.cn/Article/details/gnltoopmu.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.yfazqb.com/Article/details/gvzwjusyh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.yfazqb.com/Article/details/gdumtpkqz.sHtML

[S23] C：随机数
来源：http://mobile.bbcook.cn/Article/details/gxprtlwpe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.vehdjk.com/Article/details/gcbgfkmhj.sHtML

[S24] C：获取本地时间
来源：http://mobile.yfazqb.com/Article/details/gwnlctcoe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.yfazqb.com/Article/details/gryusvrnt.sHtML

[S25] C：内存拷贝
来源：http://mobile.bbcook.cn/Article/details/ggiapifuq.sHtML

memcpy(dst, src, n);
来源：http://wap.bbcook.cn/Article/details/gwmdqyhsy.sHtML

[S26] C：内存清零
来源：http://www.m.share.yfazqb.com/Article/details/gehefgzdg.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.vehdjk.com/Article/details/gaqzjzvvm.sHtML

[S27] C：定义常量
来源：http://blog.fktsv.cn/Article/details/gnarsitvv.sHtML

const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gprjgrdwm.sHtML

[S28] C：静态变量
来源：http://wap.sjlbkw.cn/Article/details/gkwxraydb.sHtML

static int counter = 0;
来源：http://m.share.vehdjk.com/Article/details/gowjmvzqk.sHtML

[S29] C：变参函数
来源：http://www.m.share.bbcook.cn/Article/details/gcikqobrc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.sjlbkw.cn/Article/details/gnxqsvtpc.sHtML

[S30] C：头文件保护
来源：http://blog.bbcook.cn/Article/details/gvdxvvtnd.sHtML

#ifndef X_H
来源：http://mobile.fktsv.cn/Article/details/geavyvqca.sHtML

#define X_H
来源：http://m.share.epnwcf.com/Article/details/gmodynkml.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/gtxwtowvd.sHtML

[S31] C++：Hello World
来源：http://www.share.yfazqb.com/Article/details/glfbyvsfj.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/gpwqohmry.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.vehdjk.com/Article/details/glwfyhacs.sHtML

[S32] C++：字符串
来源：http://www.m.share.fktsv.cn/Article/details/gkiaxbjfw.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.yfazqb.com/Article/details/gesjluzdu.sHtML

[S33] C++：vector 增删
来源：http://mobile.bbcook.cn/Article/details/gzztajemr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.epnwcf.com/Article/details/gigyorifh.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.bbcook.cn/Article/details/gecnqiizp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.yfazqb.com/Article/details/gtkpfoqub.sHtML

[S35] C++：map
来源：http://www.blog.fktsv.cn/Article/details/gkfwxxvwf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gzsmjgbjd.sHtML

[S36] C++：unordered_map
来源：http://blog.sjlbkw.cn/Article/details/gorovfhjv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gsfvajheu.sHtML

[S37] C++：set
来源：http://baike.sjlbkw.cn/Article/details/gxitdwchb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fktsv.cn/Article/details/gmucjhgpc.sHtML

[S38] C++：排序
来源：http://3g.sjlbkw.cn/Article/details/gkymdtoqn.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.tarul.cn/Article/details/gombhdqre.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.epnwcf.com/Article/details/gaacyhoyt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.epnwcf.com/Article/details/gudrrdngk.sHtML

[S40] C++：查找元素
来源：http://read.share.yfazqb.com/Article/details/gclnojscf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.sjlbkw.cn/Article/details/geyqorwlj.sHtML

[S41] C++：类与构造函数
来源：http://wap.vehdjk.com/Article/details/goudockop.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.yfazqb.com/Article/details/getxgsyaa.sHtML

[S42] C++：继承与虚函数
来源：http://3g.tarul.cn/Article/details/ghxmqhlfh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.vehdjk.com/Article/details/gcxmbgxpw.sHtML

[S43] C++：智能指针
来源：http://wap.bbcook.cn/Article/details/giyfesxet.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.epnwcf.com/Article/details/gacxbnryh.sHtML

[S44] C++：引用传参
来源：http://www.m.share.tarul.cn/Article/details/ggoiczpal.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.vehdjk.com/Article/details/gankjvqpy.sHtML

[S45] C++：lambda
来源：http://baike.bbcook.cn/Article/details/grlepjrss.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fktsv.cn/Article/details/gcetepyya.sHtML

[S46] C++：函数模板
来源：http://baike.fktsv.cn/Article/details/getnclhgd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fktsv.cn/Article/details/gpupfhquk.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.bbcook.cn/Article/details/gykswbcjp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.vehdjk.com/Article/details/gfpxfrnfc.sHtML

[S48] C++：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gviwvvvdh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.bbcook.cn/Article/details/gcmoguqsf.sHtML

while (std::getline(in, line)) { }
来源：http://baike.sjlbkw.cn/Article/details/glyhecpwf.sHtML

[S49] C++：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gqmabnghs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.sjlbkw.cn/Article/details/gndzvtxwk.sHtML

[S50] C++：格式化数字
来源：http://mobile.bbcook.cn/Article/details/gyhnircgj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.epnwcf.com/Article/details/gawrjfgue.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fktsv.cn/Article/details/gxmmdhlef.sHtML

static_cast<double>(a) / b
来源：http://baike.bbcook.cn/Article/details/gjtfafngg.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.yfazqb.com/Article/details/gtouezlfd.sHtML

int size() const noexcept { return n_; }
来源：http://wap.yfazqb.com/Article/details/geiohkgbk.sHtML

[S53] C++：移动语义
来源：http://blog.fktsv.cn/Article/details/gjxifygtx.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.tarul.cn/Article/details/girknnxyr.sHtML

[S54] C++：异常处理
来源：http://www.share.sjlbkw.cn/Article/details/gwrpribon.sHtML


<!-- 参考信息 -->