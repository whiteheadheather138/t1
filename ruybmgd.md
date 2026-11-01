代发 wailian999

[Q86] 读取 JSON 字段
来源：http://read.share.epnwcf.com/Article/details/gvstgimjj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.bbcook.cn/Article/details/gikmrxpdg.sHtML

[Q87] JSON 字段做条件
来源：http://baike.vehdjk.com/Article/details/ghumqkdwg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.sjlbkw.cn/Article/details/gunihwewj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.vehdjk.com/Article/details/grrppwrak.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.yfazqb.com/Article/details/gtulbgfrh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.vehdjk.com/Article/details/godjsjfwl.sHtML

[Q89] 判断表是否存在
来源：http://m.share.vehdjk.com/Article/details/grxcahewb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.yfazqb.com/Article/details/ggvaxjwyn.sHtML

[Q90] 生成序号列
来源：http://baike.tarul.cn/Article/details/guvpcdvsh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fktsv.cn/Article/details/gjhlshiwm.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gefhzvadj.sHtML

R. Bash 专题
来源：http://baike.yfazqb.com/Article/details/gjssnbkyo.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gcdpjwykm.sHtML

[R01] shebang 与严格模式
来源：http://m.share.yfazqb.com/Article/details/gauhenoyh.sHtML

#!/usr/bin/env bash
来源：http://mobile.yfazqb.com/Article/details/ggsiuqjtn.sHtML

set -euo pipefail
来源：http://www.m.share.fktsv.cn/Article/details/gvssfxtii.sHtML

[R02] 变量赋值与使用
来源：http://wap.tarul.cn/Article/details/gmwctsgtd.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.tarul.cn/Article/details/gikdwkrxk.sHtML

[R03] 只读变量
来源：http://baike.epnwcf.com/Article/details/giqsqtrau.sHtML

readonly PI=3.14
来源：http://wap.epnwcf.com/Article/details/ghjtctzaw.sHtML

[R04] 位置参数
来源：http://mobile.vehdjk.com/Article/details/gxqkyhpat.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.sjlbkw.cn/Article/details/geakwpzml.sHtML

[R05] 参数默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gzodtccqo.sHtML

name="${1:-default}"
来源：http://m.share.fktsv.cn/Article/details/gktybfnsw.sHtML

[R06] 判断命令是否存在
来源：http://3g.fktsv.cn/Article/details/gcwxuyrnh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gxxjvhcni.sHtML

[R07] if 判断文件
来源：http://www.share.vehdjk.com/Article/details/ggufyhqqb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.epnwcf.com/Article/details/gjtzjrxtd.sHtML

[R08] 数值比较
来源：http://blog.epnwcf.com/Article/details/gkglrqdjx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.bbcook.cn/Article/details/gowshsbbn.sHtML

[R09] 字符串比较
来源：http://blog.sjlbkw.cn/Article/details/gevoaazze.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.vehdjk.com/Article/details/gignstref.sHtML

[R10] 正则匹配
来源：http://baike.epnwcf.com/Article/details/gwlkqjwre.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.vehdjk.com/Article/details/gqyrigwcw.sHtML

[R11] case 多分支
来源：http://baike.sjlbkw.cn/Article/details/glncpyhtc.sHtML

case "$1" in
来源：http://mobile.fktsv.cn/Article/details/gocrnbaue.sHtML

start) echo "启动" ;;
来源：http://blog.tarul.cn/Article/details/gejzxstqf.sHtML

stop)  echo "停止" ;;
来源：http://www.share.tarul.cn/Article/details/gowihkbnp.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.tarul.cn/Article/details/gwahmfrpr.sHtML

esac
来源：http://blog.sjlbkw.cn/Article/details/guxccfdgm.sHtML

[R12] for 遍历文件
来源：http://baike.fktsv.cn/Article/details/giptfgpzu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fktsv.cn/Article/details/gyogwncpl.sHtML

[R13] for 计数循环
来源：http://blog.fktsv.cn/Article/details/gojedayry.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/gwafjminu.sHtML

[R14] C 风格 for
来源：http://www.blog.bbcook.cn/Article/details/gmkdiqjfz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gycfggudi.sHtML

[R15] while 逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gxhwpiiwc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.vehdjk.com/Article/details/gxexfomih.sHtML

[R16] until 等待条件
来源：http://www.share.sjlbkw.cn/Article/details/gllpitxty.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.yfazqb.com/Article/details/gimyqzuyv.sHtML

[R17] 数组定义与取值
来源：http://mobile.tarul.cn/Article/details/gcsxezaji.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.tarul.cn/Article/details/gtbedsuyp.sHtML

[R18] 遍历数组
来源：http://mobile.bbcook.cn/Article/details/gtnhvjdhz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.bbcook.cn/Article/details/gpipbprdt.sHtML

[R19] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/gfpbnjybp.sHtML

echo "${#arr[@]}"
来源：http://blog.bbcook.cn/Article/details/gwtlcmors.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjiezkbwx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fktsv.cn/Article/details/gqxxwbuin.sHtML

[R21] 字符串长度
来源：http://3g.yfazqb.com/Article/details/gefdqretp.sHtML

echo "${#s}"
来源：http://3g.vehdjk.com/Article/details/gtqjogcam.sHtML

[R22] 截取子串
来源：http://wap.yfazqb.com/Article/details/gylingils.sHtML

echo "${s:0:5}"
来源：http://read.share.tarul.cn/Article/details/gkwshcwvj.sHtML

[R23] 字符串替换
来源：http://3g.vehdjk.com/Article/details/gwwatvach.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.tarul.cn/Article/details/ggzqsoghp.sHtML

[R24] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gjcsghodt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fktsv.cn/Article/details/gptbbxmiq.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.yfazqb.com/Article/details/gceadjnuh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.sjlbkw.cn/Article/details/gujkgecxb.sHtML

[R26] 命令替换
来源：http://mobile.fktsv.cn/Article/details/gtjrouyno.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.vehdjk.com/Article/details/guxloapel.sHtML

[R27] 算术展开
来源：http://m.share.fktsv.cn/Article/details/grpnaiejd.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.epnwcf.com/Article/details/gygizjdwu.sHtML

[R28] 浮点运算
来源：http://read.share.yfazqb.com/Article/details/gbvafpkse.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.epnwcf.com/Article/details/gkhaqgwfs.sHtML

[R29] 定义函数
来源：http://m.share.bbcook.cn/Article/details/gjmnflvtx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.epnwcf.com/Article/details/gsspnlitj.sHtML

[R30] 函数返回状态码
来源：http://www.blog.vehdjk.com/Article/details/gmesjbdcv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.bbcook.cn/Article/details/gxuygmifs.sHtML

[R31] 局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gjgnkdcbf.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.bbcook.cn/Article/details/gtpnrfmyw.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fktsv.cn/Article/details/gfczfuznz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grzlxrwdf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.epnwcf.com/Article/details/gebmcaaum.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.sjlbkw.cn/Article/details/gnmxpyxuy.sHtML

[R34] 退出时清理
来源：http://www.m.share.vehdjk.com/Article/details/gnsxvrahx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.tarul.cn/Article/details/gznhjfila.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.bbcook.cn/Article/details/gjobxhzhm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.epnwcf.com/Article/details/gguyamzwp.sHtML

[R36] 并发执行多个任务
来源：http://www.share.vehdjk.com/Article/details/gxknpxcai.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.vehdjk.com/Article/details/gosbwjkpl.sHtML

[R37] 把输出赋给变量
来源：http://baike.fktsv.cn/Article/details/ghxmtdepb.sHtML

files=$(ls -1)
来源：http://www.share.sjlbkw.cn/Article/details/gnovsxzvf.sHtML

[R38] 管道串联
来源：http://baike.yfazqb.com/Article/details/geztokajk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.epnwcf.com/Article/details/gztsaycah.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.sjlbkw.cn/Article/details/gxtibylxw.sHtML

cmd > out.log 2>&1
来源：http://3g.tarul.cn/Article/details/giuoiotak.sHtML

[R40] 追加写日志
来源：http://blog.sjlbkw.cn/Article/details/gkjtywxlx.sHtML

echo "log" >> out.log
来源：http://3g.tarul.cn/Article/details/gpivjygsg.sHtML

[R41] 丢弃输出
来源：http://www.blog.tarul.cn/Article/details/gixnureha.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fktsv.cn/Article/details/gaawjdpdg.sHtML

[R42] 输入重定向
来源：http://mobile.sjlbkw.cn/Article/details/guqwpjgkj.sHtML

wc -l < a.txt
来源：http://wap.sjlbkw.cn/Article/details/gxpdzyjhy.sHtML

[R43] 按名字查找文件
来源：http://www.blog.sjlbkw.cn/Article/details/gqffqkrox.sHtML

find . -name "*.log" -type f
来源：http://blog.epnwcf.com/Article/details/gbqcjaula.sHtML

[R44] 按修改时间查找
来源：http://baike.tarul.cn/Article/details/gqefwlwsv.sHtML

find . -mtime -7 -type f
来源：http://read.share.bbcook.cn/Article/details/gotjwgxrw.sHtML

[R45] 批量删除
来源：http://mobile.fktsv.cn/Article/details/glqpgxwaw.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.sjlbkw.cn/Article/details/giewzsaco.sHtML

[R46] 递归替换文件内容
来源：http://wap.fktsv.cn/Article/details/gccknpufj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.vehdjk.com/Article/details/ggbiehwgv.sHtML

[R47] sed 单行替换
来源：http://mobile.fktsv.cn/Article/details/gfypcugoz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gibduekzx.sHtML

[R48] awk 取指定列
来源：http://baike.vehdjk.com/Article/details/gwteqizdr.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fktsv.cn/Article/details/gbavcnabh.sHtML

[R49] awk 带条件
来源：http://m.share.bbcook.cn/Article/details/ggqejloqz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.yfazqb.com/Article/details/gpazmrnxl.sHtML

[R50] awk 求和
来源：http://3g.yfazqb.com/Article/details/grqhgvmos.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.yfazqb.com/Article/details/gtvnjfzca.sHtML

[R51] 排序去重取前几
来源：http://www.blog.yfazqb.com/Article/details/geaeqvzlz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.yfazqb.com/Article/details/guzsgqwdx.sHtML

[R52] 统计行数
来源：http://baike.tarul.cn/Article/details/gimxnacva.sHtML

wc -l a.txt
来源：http://3g.bbcook.cn/Article/details/gfjryurxy.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.epnwcf.com/Article/details/gucabocud.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fktsv.cn/Article/details/gswzfgwqw.sHtML

[R54] 比较两个文件
来源：http://baike.sjlbkw.cn/Article/details/gsghxxhed.sHtML

diff a.txt b.txt
来源：http://www.blog.bbcook.cn/Article/details/gfirkyweq.sHtML

[R55] 压缩与解压
来源：http://m.share.sjlbkw.cn/Article/details/gnssorxdh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.yfazqb.com/Article/details/gobpyodwt.sHtML

[R56] 远程拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gqaipykai.sHtML

scp file user@host:/path/
来源：http://3g.yfazqb.com/Article/details/gvasgkbnn.sHtML

[R57] 远程执行命令
来源：http://wap.fktsv.cn/Article/details/gzpgvgiil.sHtML

ssh user@host 'uptime'
来源：http://wap.bbcook.cn/Article/details/gtdbyxoht.sHtML

[R58] 下载文件
来源：http://read.share.tarul.cn/Article/details/gcegwkjlr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.bbcook.cn/Article/details/gewtnxqtm.sHtML

[R59] 发 POST JSON
来源：http://mobile.vehdjk.com/Article/details/gmnjittqm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fktsv.cn/Article/details/gwbadlpmx.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/gwxuhgnxa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.bbcook.cn/Article/details/gwhlvdcgj.sHtML

[R61] 磁盘占用
来源：http://mobile.epnwcf.com/Article/details/goyunevrn.sHtML

df -h;  du -sh *
来源：http://wap.yfazqb.com/Article/details/gpazcylnw.sHtML

[R62] 找最占空间的文件
来源：http://3g.tarul.cn/Article/details/gurkhrjsw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.yfazqb.com/Article/details/gzppeoudh.sHtML

[R63] 内存与进程
来源：http://3g.sjlbkw.cn/Article/details/gmoowapac.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.sjlbkw.cn/Article/details/ghafpeagn.sHtML

[R64] 结束进程
来源：http://read.share.sjlbkw.cn/Article/details/gszrjrjtn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.bbcook.cn/Article/details/gqjwptwli.sHtML

[R65] 查看端口占用
来源：http://baike.bbcook.cn/Article/details/gabzgzjoo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.bbcook.cn/Article/details/ggtygmjeg.sHtML

[R66] 定时任务
来源：http://www.m.share.epnwcf.com/Article/details/glhekfteu.sHtML

crontab -e;  crontab -l
来源：http://www.share.bbcook.cn/Article/details/gciukpskk.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.sjlbkw.cn/Article/details/gvtjkhzlk.sHtML

openssl rand -hex 16
来源：http://www.m.share.fktsv.cn/Article/details/gqegceqkh.sHtML

[R68] 计算文件校验值
来源：http://read.share.tarul.cn/Article/details/gbqowrvtv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gpdzdmpwt.sHtML

[R69] 生成随机密码
来源：http://m.share.yfazqb.com/Article/details/giczewlnm.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.bbcook.cn/Article/details/gcwruzrwv.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/gmvfrfvaz.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.epnwcf.com/Article/details/gphmftmdq.sHtML

[R71] 日期格式化
来源：http://3g.bbcook.cn/Article/details/govellzxr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.epnwcf.com/Article/details/gpoonqobw.sHtML

[R72] 等待端口就绪
来源：http://wap.bbcook.cn/Article/details/gdddzmdfc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/gibfsioxf.sHtML

[R73] 分割大日志
来源：http://read.share.bbcook.cn/Article/details/gyvnsyhta.sHtML

split -l 1000 big.log part_
来源：http://read.share.vehdjk.com/Article/details/givlfvsho.sHtML

[R74] 批量重命名
来源：http://3g.tarul.cn/Article/details/gwlvehiqj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.yfazqb.com/Article/details/gutxgbnve.sHtML

[R75] 导出环境变量
来源：http://read.share.yfazqb.com/Article/details/gsrjvhtee.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fktsv.cn/Article/details/gmrmtqlwz.sHtML

[R76] 使用临时文件
来源：http://www.blog.epnwcf.com/Article/details/gnvqqvnzl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/ghifofecy.sHtML

[R77] 读取用户输入
来源：http://baike.yfazqb.com/Article/details/gjoceerzm.sHtML

read -rp "请输入: " ans
来源：http://baike.vehdjk.com/Article/details/gfvujurfb.sHtML

[R78] 交互式菜单
来源：http://www.blog.bbcook.cn/Article/details/ghzmkdjbd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.sjlbkw.cn/Article/details/gholkromi.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.vehdjk.com/Article/details/gnxthntvl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.bbcook.cn/Article/details/ggufjtrgx.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.sjlbkw.cn/Article/details/gcuvsgzgl.sHtML

time ./run.sh
来源：http://mobile.epnwcf.com/Article/details/gukhgmran.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzvhnltew.sHtML

S. C / C++ 专题
来源：http://3g.fktsv.cn/Article/details/gbeimdxin.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghmyrogrf.sHtML

[S01] C：Hello World
来源：http://wap.yfazqb.com/Article/details/gvkmixbzv.sHtML

#include <stdio.h>
来源：http://baike.tarul.cn/Article/details/gxekdrrzd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fktsv.cn/Article/details/gqaujnqbb.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcnuqvrz.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.tarul.cn/Article/details/gniybodmx.sHtML

[S03] C：读入整数
来源：http://read.share.tarul.cn/Article/details/gynhtmtns.sHtML

int x; scanf("%d", &x);
来源：http://baike.bbcook.cn/Article/details/gatzxmqlm.sHtML

[S04] C：字符串复制
来源：http://www.blog.fktsv.cn/Article/details/gbpjjijrt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.tarul.cn/Article/details/gkockwfhd.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gcsgfflai.sHtML

strlen(s)
来源：http://mobile.vehdjk.com/Article/details/grxppmshd.sHtML

[S06] C：字符串比较
来源：http://3g.vehdjk.com/Article/details/gvdpqpdpr.sHtML

strcmp(a, b) == 0
来源：http://mobile.epnwcf.com/Article/details/ggsbrfrdj.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fktsv.cn/Article/details/gfxidiyna.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.vehdjk.com/Article/details/gpxfqignx.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.yfazqb.com/Article/details/gdxuvazht.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.yfazqb.com/Article/details/ghqraxnjv.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.bbcook.cn/Article/details/ggqycnzvc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fktsv.cn/Article/details/gnpvlvepu.sHtML

[S10] C：指针与解引用
来源：http://baike.yfazqb.com/Article/details/gfxtrdofz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.vehdjk.com/Article/details/gevdshyjk.sHtML

[S11] C：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/ggjrgxrbk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.vehdjk.com/Article/details/girvwsqgk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.epnwcf.com/Article/details/gkiiglnyh.sHtML

fclose(f);
来源：http://mobile.yfazqb.com/Article/details/guknvsqwt.sHtML

[S12] C：写文件
来源：http://www.m.share.yfazqb.com/Article/details/giyvdoyft.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.bbcook.cn/Article/details/gbzfcrgoo.sHtML

[S13] C：宏定义
来源：http://m.share.vehdjk.com/Article/details/gcrilnavj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.sjlbkw.cn/Article/details/gvahssqsv.sHtML

[S14] C：枚举
来源：http://3g.sjlbkw.cn/Article/details/gkdygvvlp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.tarul.cn/Article/details/gtjylzkhf.sHtML

[S15] C：类型转换
来源：http://baike.epnwcf.com/Article/details/gucduuhqb.sHtML

(double) a / b
来源：http://www.m.share.bbcook.cn/Article/details/gefypjess.sHtML

[S16] C：位操作置位
来源：http://blog.fktsv.cn/Article/details/gchdtcjfm.sHtML

x |= (1 << 3);
来源：http://read.share.bbcook.cn/Article/details/gpbkhftpe.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gwmdhkuvx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.sjlbkw.cn/Article/details/grnixzsfe.sHtML

[S18] C：命令行参数
来源：http://3g.vehdjk.com/Article/details/gcwnjbtbp.sHtML

int main(int argc, char **argv)
来源：http://blog.bbcook.cn/Article/details/gvznezlfd.sHtML

[S19] C：快速排序
来源：http://mobile.fktsv.cn/Article/details/gijaoeuzi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.tarul.cn/Article/details/grwabgvua.sHtML

[S20] C：二分查找
来源：http://www.blog.epnwcf.com/Article/details/gftdudxzr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/gxjwdabqm.sHtML

[S21] C：字符类别判断
来源：http://mobile.sjlbkw.cn/Article/details/gowtpqbqb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.epnwcf.com/Article/details/gdpiwpynu.sHtML

[S22] C：字符串转数字
来源：http://wap.bbcook.cn/Article/details/gutarwqku.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fktsv.cn/Article/details/ghmvlmdsh.sHtML

[S23] C：随机数
来源：http://read.share.fktsv.cn/Article/details/gjygjtrfc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.tarul.cn/Article/details/gblfphpci.sHtML

[S24] C：获取本地时间
来源：http://wap.sjlbkw.cn/Article/details/gbozzrpvy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.vehdjk.com/Article/details/gmreacrev.sHtML

[S25] C：内存拷贝
来源：http://3g.sjlbkw.cn/Article/details/ghhkqpuls.sHtML

memcpy(dst, src, n);
来源：http://wap.sjlbkw.cn/Article/details/gevibufzu.sHtML

[S26] C：内存清零
来源：http://m.share.vehdjk.com/Article/details/gagnnarpp.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.yfazqb.com/Article/details/gyjhmqgpn.sHtML

[S27] C：定义常量
来源：http://wap.epnwcf.com/Article/details/gebanseop.sHtML

const double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gzrkaqwdh.sHtML

[S28] C：静态变量
来源：http://www.share.vehdjk.com/Article/details/gpubqarss.sHtML

static int counter = 0;
来源：http://blog.bbcook.cn/Article/details/gwkhonmbd.sHtML

[S29] C：变参函数
来源：http://baike.yfazqb.com/Article/details/gaazytjkk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fktsv.cn/Article/details/grpkhbotl.sHtML

[S30] C：头文件保护
来源：http://blog.tarul.cn/Article/details/gnvsywptv.sHtML

#ifndef X_H
来源：http://mobile.fktsv.cn/Article/details/gyoshvqpi.sHtML

#define X_H
来源：http://www.share.vehdjk.com/Article/details/gmbfjfrpr.sHtML

#endif
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkbcvind.sHtML

[S31] C++：Hello World
来源：http://baike.fktsv.cn/Article/details/gaxdugkpq.sHtML

#include <iostream>
来源：http://m.share.epnwcf.com/Article/details/gxmscebml.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.vehdjk.com/Article/details/gbisghqeh.sHtML

[S32] C++：字符串
来源：http://baike.sjlbkw.cn/Article/details/gqktvypdy.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fktsv.cn/Article/details/gtcavsmkk.sHtML

[S33] C++：vector 增删
来源：http://m.share.yfazqb.com/Article/details/ggtkjpemz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.sjlbkw.cn/Article/details/gsjqpmpxn.sHtML

[S34] C++：遍历 vector
来源：http://mobile.bbcook.cn/Article/details/gabdnyoyh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/gmgwseokw.sHtML

[S35] C++：map
来源：http://baike.sjlbkw.cn/Article/details/gcucjlzvt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gfvsfklmo.sHtML

[S36] C++：unordered_map
来源：http://wap.yfazqb.com/Article/details/gyygeawpq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.epnwcf.com/Article/details/grkrodvzj.sHtML

[S37] C++：set
来源：http://www.share.tarul.cn/Article/details/govzpypmn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.epnwcf.com/Article/details/grsfmruhs.sHtML

[S38] C++：排序
来源：http://m.share.vehdjk.com/Article/details/gnzwhagiw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/gxddjwpfp.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.sjlbkw.cn/Article/details/gwlwcubnz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fktsv.cn/Article/details/glhvfiabw.sHtML

[S40] C++：查找元素
来源：http://baike.fktsv.cn/Article/details/gwlwunzvx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.tarul.cn/Article/details/gipxyiabe.sHtML

[S41] C++：类与构造函数
来源：http://3g.sjlbkw.cn/Article/details/gjrlrjpmh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.bbcook.cn/Article/details/giqcjdwyf.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.tarul.cn/Article/details/gajrqaazz.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fktsv.cn/Article/details/gvfnfabdp.sHtML

[S43] C++：智能指针
来源：http://3g.sjlbkw.cn/Article/details/gxsanijxe.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.yfazqb.com/Article/details/gdpjgpbjx.sHtML

[S44] C++：引用传参
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgtjhhxm.sHtML

void inc(int &x) { ++x; }
来源：http://baike.sjlbkw.cn/Article/details/gqdcxyjck.sHtML

[S45] C++：lambda
来源：http://www.blog.yfazqb.com/Article/details/ggakzuogm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fktsv.cn/Article/details/grdvqhfld.sHtML

[S46] C++：函数模板
来源：http://3g.yfazqb.com/Article/details/ggdgapbau.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.tarul.cn/Article/details/glbzgediu.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.yfazqb.com/Article/details/gnmiagkjz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fktsv.cn/Article/details/gurgjbikk.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gectjjora.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.bbcook.cn/Article/details/gumdhxiyp.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fktsv.cn/Article/details/gacsxujie.sHtML

[S49] C++：写文件
来源：http://3g.vehdjk.com/Article/details/guvfkhrxc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.yfazqb.com/Article/details/gchgppnfp.sHtML

[S50] C++：格式化数字
来源：http://baike.vehdjk.com/Article/details/gpoveedux.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.tarul.cn/Article/details/ghmdmqbbe.sHtML

[S51] C++：显式类型转换
来源：http://read.share.epnwcf.com/Article/details/gznjrsxxx.sHtML

static_cast<double>(a) / b
来源：http://read.share.sjlbkw.cn/Article/details/gpmxrxnee.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.yfazqb.com/Article/details/gbnitrgat.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.sjlbkw.cn/Article/details/giwimsjpw.sHtML

[S53] C++：移动语义
来源：http://3g.tarul.cn/Article/details/gvkmewrmp.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.yfazqb.com/Article/details/gzmybwdaf.sHtML

[S54] C++：异常处理
来源：http://read.share.yfazqb.com/Article/details/gsfnfuoyu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.tarul.cn/Article/details/gqgqwxgak.sHtML

[S55] C++：结构化绑定
来源：http://read.share.bbcook.cn/Article/details/gejxpcwsr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.vehdjk.com/Article/details/guuviyiqn.sHtML

[S56] C++：optional
来源：http://www.m.share.tarul.cn/Article/details/glyqchcjh.sHtML


<!-- 参考信息 -->