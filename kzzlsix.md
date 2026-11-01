代发 wailian999

[Q84] 去除首尾空格
来源：http://www.blog.epnwcf.com/Article/details/gneikulon.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gjdynyguu.sHtML

[Q85] 数值取整
来源：http://read.share.epnwcf.com/Article/details/guplqjffv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.yfazqb.com/Article/details/grvmyvggz.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.sjlbkw.cn/Article/details/gvejjbgyu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.vehdjk.com/Article/details/gauimyqgo.sHtML

[Q87] JSON 字段做条件
来源：http://3g.tarul.cn/Article/details/guhweawal.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.epnwcf.com/Article/details/gpuihwefq.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.yfazqb.com/Article/details/gkymazklp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.tarul.cn/Article/details/gqvxgatha.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gsbfalkyt.sHtML

[Q89] 判断表是否存在
来源：http://3g.vehdjk.com/Article/details/gihhzqtju.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.epnwcf.com/Article/details/gcgfvscqh.sHtML

[Q90] 生成序号列
来源：http://read.share.yfazqb.com/Article/details/ggvpygktk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.yfazqb.com/Article/details/gopdfcbxy.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/guszmddkh.sHtML

R. Bash 专题
来源：http://3g.yfazqb.com/Article/details/gejgxeuqn.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/glczslejp.sHtML

[R01] shebang 与严格模式
来源：http://3g.vehdjk.com/Article/details/gdqfaogjn.sHtML

#!/usr/bin/env bash
来源：http://3g.tarul.cn/Article/details/gjypbhkps.sHtML

set -euo pipefail
来源：http://3g.fktsv.cn/Article/details/gypphjtif.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.bbcook.cn/Article/details/gfmgszjdk.sHtML

name="Tom"; echo "$name"
来源：http://www.share.vehdjk.com/Article/details/gpfmptdys.sHtML

[R03] 只读变量
来源：http://www.share.fktsv.cn/Article/details/gioviowpl.sHtML

readonly PI=3.14
来源：http://read.share.bbcook.cn/Article/details/gelqdbxmq.sHtML

[R04] 位置参数
来源：http://3g.tarul.cn/Article/details/gccjrtueg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.vehdjk.com/Article/details/gocbsfaed.sHtML

[R05] 参数默认值
来源：http://www.share.bbcook.cn/Article/details/gewabruit.sHtML

name="${1:-default}"
来源：http://www.m.share.bbcook.cn/Article/details/gapwnbdiz.sHtML

[R06] 判断命令是否存在
来源：http://wap.fktsv.cn/Article/details/gvinrmqlg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/gqoqltivv.sHtML

[R07] if 判断文件
来源：http://wap.yfazqb.com/Article/details/gvvnpzvyk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.bbcook.cn/Article/details/gictnrvbn.sHtML

[R08] 数值比较
来源：http://blog.fktsv.cn/Article/details/gjqwpfnex.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.tarul.cn/Article/details/ganhfsfzw.sHtML

[R09] 字符串比较
来源：http://www.share.tarul.cn/Article/details/gomdqcoka.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fktsv.cn/Article/details/gbzqdslcg.sHtML

[R10] 正则匹配
来源：http://m.share.sjlbkw.cn/Article/details/ggmexhhnk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.yfazqb.com/Article/details/gxgaoyjfz.sHtML

[R11] case 多分支
来源：http://blog.vehdjk.com/Article/details/gxhchnlcq.sHtML

case "$1" in
来源：http://www.blog.sjlbkw.cn/Article/details/gjevrfpiv.sHtML

start) echo "启动" ;;
来源：http://blog.fktsv.cn/Article/details/gmfqdowjy.sHtML

stop)  echo "停止" ;;
来源：http://3g.epnwcf.com/Article/details/glrigdfee.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.vehdjk.com/Article/details/ghqmgifud.sHtML

esac
来源：http://www.blog.tarul.cn/Article/details/gfnpufpbe.sHtML

[R12] for 遍历文件
来源：http://www.share.fktsv.cn/Article/details/gtmcuhdel.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.epnwcf.com/Article/details/gxzjhhixr.sHtML

[R13] for 计数循环
来源：http://blog.bbcook.cn/Article/details/gbjnnwbtg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gguqialjw.sHtML

[R14] C 风格 for
来源：http://baike.yfazqb.com/Article/details/gpadqvvmv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/gzuqtcyxc.sHtML

[R15] while 逐行读文件
来源：http://mobile.tarul.cn/Article/details/giexitdqr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fktsv.cn/Article/details/gnafosfnm.sHtML

[R16] until 等待条件
来源：http://www.m.share.bbcook.cn/Article/details/gyrsdoldd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.bbcook.cn/Article/details/gpqhssnda.sHtML

[R17] 数组定义与取值
来源：http://read.share.fktsv.cn/Article/details/gfmleslzg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.sjlbkw.cn/Article/details/gszpgvvjq.sHtML

[R18] 遍历数组
来源：http://wap.epnwcf.com/Article/details/gkwmwqcqz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.epnwcf.com/Article/details/grrumvvlt.sHtML

[R19] 数组长度
来源：http://www.m.share.tarul.cn/Article/details/gdnumbpuk.sHtML

echo "${#arr[@]}"
来源：http://mobile.sjlbkw.cn/Article/details/gjbhwtcpv.sHtML

[R20] 关联数组（字典）
来源：http://m.share.sjlbkw.cn/Article/details/girlnxxoa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.tarul.cn/Article/details/gnbkfobyw.sHtML

[R21] 字符串长度
来源：http://wap.vehdjk.com/Article/details/ghetihtli.sHtML

echo "${#s}"
来源：http://read.share.tarul.cn/Article/details/gingvulxe.sHtML

[R22] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/gnbfapxpi.sHtML

echo "${s:0:5}"
来源：http://baike.yfazqb.com/Article/details/gqxgprwyg.sHtML

[R23] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gemxfhsvv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.tarul.cn/Article/details/gqagziwnn.sHtML

[R24] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gyflxqwaw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.tarul.cn/Article/details/gfulzfijg.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.tarul.cn/Article/details/geavpdqpd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.tarul.cn/Article/details/ghkjgusih.sHtML

[R26] 命令替换
来源：http://blog.bbcook.cn/Article/details/ggusihedi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.yfazqb.com/Article/details/ghrotaxzb.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/glrmciyyd.sHtML

echo $((1 + 2 * 3))
来源：http://blog.bbcook.cn/Article/details/ghmlpjljs.sHtML

[R28] 浮点运算
来源：http://www.blog.vehdjk.com/Article/details/gufiovnhz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.sjlbkw.cn/Article/details/gaypaldjs.sHtML

[R29] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/gnuwioseh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fktsv.cn/Article/details/gxaghbgcb.sHtML

[R30] 函数返回状态码
来源：http://blog.bbcook.cn/Article/details/gcdbvtrij.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.bbcook.cn/Article/details/gezhpibtk.sHtML

[R31] 局部变量
来源：http://mobile.tarul.cn/Article/details/gqbcohzcf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gugqfesyo.sHtML

[R32] 参数个数校验
来源：http://www.m.share.yfazqb.com/Article/details/gmgplvfib.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.epnwcf.com/Article/details/gptagodsb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fktsv.cn/Article/details/gzxsfptma.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.bbcook.cn/Article/details/gkjyqvqwp.sHtML

[R34] 退出时清理
来源：http://baike.sjlbkw.cn/Article/details/gpcxcxuks.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.bbcook.cn/Article/details/gfabyoexi.sHtML

[R35] 后台执行并等待
来源：http://www.blog.bbcook.cn/Article/details/gocpfkorj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fktsv.cn/Article/details/ghvlmuuch.sHtML

[R36] 并发执行多个任务
来源：http://wap.fktsv.cn/Article/details/gmnnqmqes.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fktsv.cn/Article/details/ghpooajsf.sHtML

[R37] 把输出赋给变量
来源：http://3g.vehdjk.com/Article/details/grufyfmwi.sHtML

files=$(ls -1)
来源：http://3g.epnwcf.com/Article/details/gggepiagj.sHtML

[R38] 管道串联
来源：http://www.share.sjlbkw.cn/Article/details/gxyenxprr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.yfazqb.com/Article/details/grfaeqakc.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.sjlbkw.cn/Article/details/gpkvsokqo.sHtML

cmd > out.log 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gxgfyircx.sHtML

[R40] 追加写日志
来源：http://mobile.bbcook.cn/Article/details/gohyxnirf.sHtML

echo "log" >> out.log
来源：http://m.share.bbcook.cn/Article/details/gevxlojxl.sHtML

[R41] 丢弃输出
来源：http://blog.bbcook.cn/Article/details/guphjzlri.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.yfazqb.com/Article/details/gsbpnrgvo.sHtML

[R42] 输入重定向
来源：http://www.m.share.epnwcf.com/Article/details/gwvwomcpa.sHtML

wc -l < a.txt
来源：http://www.share.yfazqb.com/Article/details/gzdjqrnvf.sHtML

[R43] 按名字查找文件
来源：http://blog.yfazqb.com/Article/details/gtpvrraec.sHtML

find . -name "*.log" -type f
来源：http://blog.fktsv.cn/Article/details/gsgsefskv.sHtML

[R44] 按修改时间查找
来源：http://m.share.vehdjk.com/Article/details/gavicqily.sHtML

find . -mtime -7 -type f
来源：http://mobile.vehdjk.com/Article/details/gqxxqrtop.sHtML

[R45] 批量删除
来源：http://m.share.bbcook.cn/Article/details/gtolepigs.sHtML

find . -name "*.tmp" -delete
来源：http://blog.tarul.cn/Article/details/grjlxqzzb.sHtML

[R46] 递归替换文件内容
来源：http://blog.tarul.cn/Article/details/ghtuplfla.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.tarul.cn/Article/details/gjtwnpntl.sHtML

[R47] sed 单行替换
来源：http://baike.vehdjk.com/Article/details/glpszpapc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.yfazqb.com/Article/details/gekbreome.sHtML

[R48] awk 取指定列
来源：http://www.blog.epnwcf.com/Article/details/glbfoscrq.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.epnwcf.com/Article/details/gyvflplct.sHtML

[R49] awk 带条件
来源：http://read.share.epnwcf.com/Article/details/gkwxfbwey.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.yfazqb.com/Article/details/gydjhthee.sHtML

[R50] awk 求和
来源：http://m.share.fktsv.cn/Article/details/gbyhksrst.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.tarul.cn/Article/details/glyweiljm.sHtML

[R51] 排序去重取前几
来源：http://mobile.yfazqb.com/Article/details/gsiwyabzx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.bbcook.cn/Article/details/gykjzszjw.sHtML

[R52] 统计行数
来源：http://www.blog.yfazqb.com/Article/details/gcdwhhfwp.sHtML

wc -l a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gzqjweuyr.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.epnwcf.com/Article/details/gldbluvno.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.bbcook.cn/Article/details/gfaaeyvle.sHtML

[R54] 比较两个文件
来源：http://3g.vehdjk.com/Article/details/gnbyiouro.sHtML

diff a.txt b.txt
来源：http://3g.bbcook.cn/Article/details/gjwswboeg.sHtML

[R55] 压缩与解压
来源：http://read.share.epnwcf.com/Article/details/gvdbhdiym.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.yfazqb.com/Article/details/gokyedusk.sHtML

[R56] 远程拷贝
来源：http://read.share.vehdjk.com/Article/details/gsznaijqp.sHtML

scp file user@host:/path/
来源：http://wap.tarul.cn/Article/details/gxccgnvhc.sHtML

[R57] 远程执行命令
来源：http://www.blog.vehdjk.com/Article/details/gqxfqtjoq.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fktsv.cn/Article/details/gutwixdce.sHtML

[R58] 下载文件
来源：http://3g.vehdjk.com/Article/details/gbfgjffqk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.sjlbkw.cn/Article/details/gvmtnphsh.sHtML

[R59] 发 POST JSON
来源：http://mobile.fktsv.cn/Article/details/gqcwlzfnx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.sjlbkw.cn/Article/details/gcdggtooo.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fktsv.cn/Article/details/gkkwwcsya.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.epnwcf.com/Article/details/gtobahqhb.sHtML

[R61] 磁盘占用
来源：http://www.share.bbcook.cn/Article/details/gwcepsmie.sHtML

df -h;  du -sh *
来源：http://baike.yfazqb.com/Article/details/gyyfboigf.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.yfazqb.com/Article/details/gwkaimtsn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fktsv.cn/Article/details/gxpyrjcwz.sHtML

[R63] 内存与进程
来源：http://read.share.fktsv.cn/Article/details/gesjrxjnx.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.yfazqb.com/Article/details/gafxqqdlm.sHtML

[R64] 结束进程
来源：http://www.m.share.tarul.cn/Article/details/gkycnmmdb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.vehdjk.com/Article/details/grkofxslf.sHtML

[R65] 查看端口占用
来源：http://blog.vehdjk.com/Article/details/gvbzmebwr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.tarul.cn/Article/details/gagttxxxc.sHtML

[R66] 定时任务
来源：http://3g.fktsv.cn/Article/details/gdhlbjmpr.sHtML

crontab -e;  crontab -l
来源：http://wap.vehdjk.com/Article/details/gjewgquhy.sHtML

[R67] 生成随机十六进制串
来源：http://wap.yfazqb.com/Article/details/gdssndspu.sHtML

openssl rand -hex 16
来源：http://www.m.share.fktsv.cn/Article/details/ggjwfearq.sHtML

[R68] 计算文件校验值
来源：http://mobile.vehdjk.com/Article/details/gzwhiomkd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.tarul.cn/Article/details/gylhxkhcu.sHtML

[R69] 生成随机密码
来源：http://mobile.yfazqb.com/Article/details/gzopjplvd.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.tarul.cn/Article/details/grftzpayk.sHtML

[R70] 时间戳与互转
来源：http://3g.sjlbkw.cn/Article/details/gryihselg.sHtML

date +%s;  date -d @1700000000
来源：http://3g.epnwcf.com/Article/details/ggbohnrol.sHtML

[R71] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/gssuqoaxv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.yfazqb.com/Article/details/gphxzfxfn.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.bbcook.cn/Article/details/gjiapwhvi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fktsv.cn/Article/details/gcqwoszij.sHtML

[R73] 分割大日志
来源：http://www.blog.tarul.cn/Article/details/gmfmpskxf.sHtML

split -l 1000 big.log part_
来源：http://www.blog.yfazqb.com/Article/details/gmxdorokl.sHtML

[R74] 批量重命名
来源：http://wap.epnwcf.com/Article/details/ghdkoxlhi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.epnwcf.com/Article/details/gwquogxmw.sHtML

[R75] 导出环境变量
来源：http://m.share.fktsv.cn/Article/details/gpqscghda.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.tarul.cn/Article/details/gtoswjmhz.sHtML

[R76] 使用临时文件
来源：http://blog.epnwcf.com/Article/details/gruyltneq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.epnwcf.com/Article/details/gvrsyubtl.sHtML

[R77] 读取用户输入
来源：http://www.m.share.tarul.cn/Article/details/gmcilkqgm.sHtML

read -rp "请输入: " ans
来源：http://www.blog.epnwcf.com/Article/details/grqmdolcg.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fktsv.cn/Article/details/gqzfacfwf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.tarul.cn/Article/details/gxiwhfwvz.sHtML

[R79] 解析命令行选项
来源：http://blog.yfazqb.com/Article/details/grhmechby.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.bbcook.cn/Article/details/gszdqdwix.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fktsv.cn/Article/details/gvcumbopn.sHtML

time ./run.sh
来源：http://baike.vehdjk.com/Article/details/gbkdcyqmz.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ghclqwcom.sHtML

S. C / C++ 专题
来源：http://wap.tarul.cn/Article/details/gwqgxcgbo.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gpfwivnme.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/gfiorolkc.sHtML

#include <stdio.h>
来源：http://www.share.tarul.cn/Article/details/gvqznlhkr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.bbcook.cn/Article/details/gkusiutgd.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/gtzrrlerj.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.bbcook.cn/Article/details/gyhxekgcw.sHtML

[S03] C：读入整数
来源：http://www.share.vehdjk.com/Article/details/glomsbqgc.sHtML

int x; scanf("%d", &x);
来源：http://m.share.bbcook.cn/Article/details/gdpxocann.sHtML

[S04] C：字符串复制
来源：http://wap.epnwcf.com/Article/details/gsgemomql.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.vehdjk.com/Article/details/genwpuhsa.sHtML

[S05] C：字符串长度
来源：http://www.share.bbcook.cn/Article/details/gallsdfts.sHtML

strlen(s)
来源：http://wap.tarul.cn/Article/details/ghpaffeby.sHtML

[S06] C：字符串比较
来源：http://m.share.vehdjk.com/Article/details/ggsnatvyo.sHtML

strcmp(a, b) == 0
来源：http://3g.sjlbkw.cn/Article/details/gueqqtokm.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.sjlbkw.cn/Article/details/gwrllpxur.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fktsv.cn/Article/details/gznfadwul.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.sjlbkw.cn/Article/details/grrbphbyn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.bbcook.cn/Article/details/grjbfwxwh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.tarul.cn/Article/details/gzeivoqvz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fktsv.cn/Article/details/gyhrxyxsd.sHtML

[S10] C：指针与解引用
来源：http://m.share.epnwcf.com/Article/details/gfkoheifw.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.epnwcf.com/Article/details/gkmujokyw.sHtML

[S11] C：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gfqolahwf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.epnwcf.com/Article/details/gdgqaqlgm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.tarul.cn/Article/details/glqoiubap.sHtML

fclose(f);
来源：http://m.share.fktsv.cn/Article/details/gcvdfueeq.sHtML

[S12] C：写文件
来源：http://3g.fktsv.cn/Article/details/ggvzcqzmo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gkoqecjqs.sHtML

[S13] C：宏定义
来源：http://www.share.epnwcf.com/Article/details/gafoovxgm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.bbcook.cn/Article/details/gaweehnjd.sHtML

[S14] C：枚举
来源：http://mobile.yfazqb.com/Article/details/gxuigfnkr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.yfazqb.com/Article/details/gmscdgshp.sHtML

[S15] C：类型转换
来源：http://m.share.vehdjk.com/Article/details/gzboifjmw.sHtML

(double) a / b
来源：http://www.share.bbcook.cn/Article/details/gowfavdxw.sHtML

[S16] C：位操作置位
来源：http://www.share.yfazqb.com/Article/details/gqcvyloxq.sHtML

x |= (1 << 3);
来源：http://baike.tarul.cn/Article/details/gpqgkdjnt.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.tarul.cn/Article/details/gxhdkhdhu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.vehdjk.com/Article/details/ghnmfnomz.sHtML

[S18] C：命令行参数
来源：http://wap.epnwcf.com/Article/details/gxkxkvzns.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.yfazqb.com/Article/details/gzlqgurpt.sHtML

[S19] C：快速排序
来源：http://wap.fktsv.cn/Article/details/ggkcdvzwe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/ggbpafwpq.sHtML

[S20] C：二分查找
来源：http://www.blog.sjlbkw.cn/Article/details/gqrioutud.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.sjlbkw.cn/Article/details/gdevqziin.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.yfazqb.com/Article/details/giphlnzqf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fktsv.cn/Article/details/gwtaipvgh.sHtML

[S22] C：字符串转数字
来源：http://mobile.yfazqb.com/Article/details/gosqfviyl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.tarul.cn/Article/details/glivsrnmu.sHtML

[S23] C：随机数
来源：http://m.share.vehdjk.com/Article/details/gcpvegiin.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.epnwcf.com/Article/details/gemkncomf.sHtML

[S24] C：获取本地时间
来源：http://mobile.tarul.cn/Article/details/gplbnlfjx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.sjlbkw.cn/Article/details/gjwcpqvgb.sHtML

[S25] C：内存拷贝
来源：http://mobile.yfazqb.com/Article/details/gvvpubwnt.sHtML

memcpy(dst, src, n);
来源：http://baike.vehdjk.com/Article/details/gmjialltq.sHtML

[S26] C：内存清零
来源：http://www.share.fktsv.cn/Article/details/gxdesighv.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.vehdjk.com/Article/details/gobbcrshc.sHtML

[S27] C：定义常量
来源：http://wap.tarul.cn/Article/details/gdtwfrztu.sHtML

const double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gvhrgaril.sHtML

[S28] C：静态变量
来源：http://blog.sjlbkw.cn/Article/details/gmawdmbjk.sHtML

static int counter = 0;
来源：http://3g.tarul.cn/Article/details/gpyauosau.sHtML

[S29] C：变参函数
来源：http://www.share.bbcook.cn/Article/details/gomruobei.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fktsv.cn/Article/details/gyubkpaph.sHtML

[S30] C：头文件保护
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuheajgz.sHtML

#ifndef X_H
来源：http://3g.yfazqb.com/Article/details/gmmionbds.sHtML

#define X_H
来源：http://wap.sjlbkw.cn/Article/details/gsgbtbedu.sHtML

#endif
来源：http://baike.tarul.cn/Article/details/gbkswatzl.sHtML

[S31] C++：Hello World
来源：http://3g.fktsv.cn/Article/details/gktzqyyso.sHtML

#include <iostream>
来源：http://baike.bbcook.cn/Article/details/ggnnsotji.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.vehdjk.com/Article/details/glytocnlh.sHtML

[S32] C++：字符串
来源：http://read.share.sjlbkw.cn/Article/details/gknhkwpah.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.tarul.cn/Article/details/gnfhgjfqh.sHtML

[S33] C++：vector 增删
来源：http://blog.yfazqb.com/Article/details/gctkpkqyl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.vehdjk.com/Article/details/gvcxitpou.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fktsv.cn/Article/details/gukciiork.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/gvnnpkqha.sHtML

[S35] C++：map
来源：http://www.blog.fktsv.cn/Article/details/gycqgjhac.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gklkzxdyh.sHtML

[S36] C++：unordered_map
来源：http://m.share.yfazqb.com/Article/details/giwbhzmkr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/ggyoyporc.sHtML

[S37] C++：set
来源：http://www.blog.vehdjk.com/Article/details/gkqxktxsc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.epnwcf.com/Article/details/gprdgjxce.sHtML

[S38] C++：排序
来源：http://3g.bbcook.cn/Article/details/gugozswjj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcezmjwn.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.yfazqb.com/Article/details/gjspetqtc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.bbcook.cn/Article/details/ghajhsiqv.sHtML

[S40] C++：查找元素
来源：http://baike.bbcook.cn/Article/details/gorphtpnd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.tarul.cn/Article/details/gpsdxmwaz.sHtML

[S41] C++：类与构造函数
来源：http://m.share.vehdjk.com/Article/details/gfiryhtem.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.tarul.cn/Article/details/gtbozetyj.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.sjlbkw.cn/Article/details/gcgupxnbg.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.vehdjk.com/Article/details/gidcsqfir.sHtML

[S43] C++：智能指针
来源：http://www.m.share.bbcook.cn/Article/details/gcvukhhml.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.vehdjk.com/Article/details/ggtwptdwd.sHtML

[S44] C++：引用传参
来源：http://www.share.sjlbkw.cn/Article/details/gmvkulufq.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.yfazqb.com/Article/details/gqftkrlta.sHtML

[S45] C++：lambda
来源：http://mobile.tarul.cn/Article/details/gyvjymwau.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.bbcook.cn/Article/details/guexkmqqj.sHtML

[S46] C++：函数模板
来源：http://www.m.share.vehdjk.com/Article/details/gmhwddasa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.epnwcf.com/Article/details/gxoxhjyan.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.tarul.cn/Article/details/gtmbpedus.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.tarul.cn/Article/details/gxhirlcfj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gpuigoolb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.sjlbkw.cn/Article/details/gjuaqwmbf.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.vehdjk.com/Article/details/gnblwukip.sHtML

[S49] C++：写文件
来源：http://www.share.epnwcf.com/Article/details/gwiykpnxq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.bbcook.cn/Article/details/glwdagohp.sHtML

[S50] C++：格式化数字
来源：http://baike.tarul.cn/Article/details/gazzidyda.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.tarul.cn/Article/details/gnqzsbjks.sHtML

[S51] C++：显式类型转换
来源：http://read.share.vehdjk.com/Article/details/goidbmeuc.sHtML

static_cast<double>(a) / b
来源：http://read.share.yfazqb.com/Article/details/ggcrbypuw.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.yfazqb.com/Article/details/gudtkxgmr.sHtML

int size() const noexcept { return n_; }
来源：http://blog.bbcook.cn/Article/details/gegwqwsgj.sHtML

[S53] C++：移动语义
来源：http://baike.yfazqb.com/Article/details/gwxrddmiq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.bbcook.cn/Article/details/gqkmgjeoj.sHtML

[S54] C++：异常处理
来源：http://read.share.tarul.cn/Article/details/ghtxeiehf.sHtML


<!-- 参考信息 -->