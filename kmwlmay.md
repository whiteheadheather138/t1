代发 wailian999

[Q82] 字符长度与字节长度
来源：http://baike.vehdjk.com/Article/details/ginhpltit.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gslrgzazy.sHtML

[Q83] 大小写转换
来源：http://mobile.epnwcf.com/Article/details/gjkxfhyem.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gywdysiiw.sHtML

[Q84] 去除首尾空格
来源：http://3g.fktsv.cn/Article/details/gtsapwpgp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gfrpyvxfm.sHtML

[Q85] 数值取整
来源：http://www.share.vehdjk.com/Article/details/ghsmwqniq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.epnwcf.com/Article/details/gqltwvkhh.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.yfazqb.com/Article/details/gesalqdzt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.tarul.cn/Article/details/gsblcnwru.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.vehdjk.com/Article/details/gxzimmoqx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fktsv.cn/Article/details/gglnxpzoy.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.tarul.cn/Article/details/gnlzvuxoy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.epnwcf.com/Article/details/gvqiaswwa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gjeromeeo.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fktsv.cn/Article/details/ggcyodprv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.sjlbkw.cn/Article/details/ggltbqlne.sHtML

[Q90] 生成序号列
来源：http://www.blog.sjlbkw.cn/Article/details/gyxsgpuue.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.vehdjk.com/Article/details/gibgrlpku.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gfktrwmdg.sHtML

R. Bash 专题
来源：http://www.blog.yfazqb.com/Article/details/gayabsfic.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gywmbcoox.sHtML

[R01] shebang 与严格模式
来源：http://mobile.bbcook.cn/Article/details/gblzxvocq.sHtML

#!/usr/bin/env bash
来源：http://read.share.sjlbkw.cn/Article/details/gapcntgwq.sHtML

set -euo pipefail
来源：http://baike.fktsv.cn/Article/details/geompfcuu.sHtML

[R02] 变量赋值与使用
来源：http://mobile.bbcook.cn/Article/details/gntrcpncn.sHtML

name="Tom"; echo "$name"
来源：http://blog.sjlbkw.cn/Article/details/gzbfflmen.sHtML

[R03] 只读变量
来源：http://baike.sjlbkw.cn/Article/details/glsprwdtj.sHtML

readonly PI=3.14
来源：http://mobile.vehdjk.com/Article/details/grarjusiq.sHtML

[R04] 位置参数
来源：http://www.m.share.epnwcf.com/Article/details/gocznvvzc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.vehdjk.com/Article/details/gqrmubsxe.sHtML

[R05] 参数默认值
来源：http://blog.vehdjk.com/Article/details/gtwtkvizl.sHtML

name="${1:-default}"
来源：http://baike.yfazqb.com/Article/details/gsmjyyrnx.sHtML

[R06] 判断命令是否存在
来源：http://mobile.vehdjk.com/Article/details/gnmeqntof.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.epnwcf.com/Article/details/gwzxeywof.sHtML

[R07] if 判断文件
来源：http://mobile.sjlbkw.cn/Article/details/gxjfanzzf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.epnwcf.com/Article/details/gbdmcrbcz.sHtML

[R08] 数值比较
来源：http://blog.vehdjk.com/Article/details/gindmaqyj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.vehdjk.com/Article/details/gxfypyapc.sHtML

[R09] 字符串比较
来源：http://read.share.epnwcf.com/Article/details/gnoazvnbb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fktsv.cn/Article/details/gtequxxmy.sHtML

[R10] 正则匹配
来源：http://blog.bbcook.cn/Article/details/gxczqsykc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.vehdjk.com/Article/details/gqywevwvr.sHtML

[R11] case 多分支
来源：http://baike.tarul.cn/Article/details/gtsxhgoyh.sHtML

case "$1" in
来源：http://read.share.fktsv.cn/Article/details/gxopqtxig.sHtML

start) echo "启动" ;;
来源：http://read.share.bbcook.cn/Article/details/gwvacgvul.sHtML

stop)  echo "停止" ;;
来源：http://wap.tarul.cn/Article/details/gldgppitv.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fktsv.cn/Article/details/gkexcigis.sHtML

esac
来源：http://www.blog.epnwcf.com/Article/details/grycrtfqz.sHtML

[R12] for 遍历文件
来源：http://m.share.vehdjk.com/Article/details/gemjglibi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gxegzvfmu.sHtML

[R13] for 计数循环
来源：http://mobile.epnwcf.com/Article/details/gyvojgdyg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.yfazqb.com/Article/details/gkabsteka.sHtML

[R14] C 风格 for
来源：http://blog.sjlbkw.cn/Article/details/gwrpzewlx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gtuncizkm.sHtML

[R15] while 逐行读文件
来源：http://baike.vehdjk.com/Article/details/gmfkxilvc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.epnwcf.com/Article/details/gpebsrvjl.sHtML

[R16] until 等待条件
来源：http://blog.vehdjk.com/Article/details/gfhpriquv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.yfazqb.com/Article/details/gxuylmnoa.sHtML

[R17] 数组定义与取值
来源：http://blog.epnwcf.com/Article/details/grambtjmz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.tarul.cn/Article/details/gpqgspxts.sHtML

[R18] 遍历数组
来源：http://read.share.fktsv.cn/Article/details/gxmrhpwoz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.vehdjk.com/Article/details/gosronexv.sHtML

[R19] 数组长度
来源：http://baike.bbcook.cn/Article/details/gqsglxlkf.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fktsv.cn/Article/details/gxtxwzhdt.sHtML

[R20] 关联数组（字典）
来源：http://wap.yfazqb.com/Article/details/gqrjqvnce.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.yfazqb.com/Article/details/gmegpowur.sHtML

[R21] 字符串长度
来源：http://read.share.fktsv.cn/Article/details/gpnlioopg.sHtML

echo "${#s}"
来源：http://m.share.vehdjk.com/Article/details/gbiamgfwu.sHtML

[R22] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gtezzehqb.sHtML

echo "${s:0:5}"
来源：http://baike.sjlbkw.cn/Article/details/gwiplyxqe.sHtML

[R23] 字符串替换
来源：http://mobile.tarul.cn/Article/details/gwjtznrgk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.sjlbkw.cn/Article/details/gdujkfgan.sHtML

[R24] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gygklhlch.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fktsv.cn/Article/details/gxuhedvgo.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.tarul.cn/Article/details/gciwmiyva.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.vehdjk.com/Article/details/gkblvnlgl.sHtML

[R26] 命令替换
来源：http://m.share.epnwcf.com/Article/details/gihaxnsul.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.sjlbkw.cn/Article/details/gkhdysyfe.sHtML

[R27] 算术展开
来源：http://www.m.share.yfazqb.com/Article/details/gjcbzezko.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.epnwcf.com/Article/details/gwmyziibk.sHtML

[R28] 浮点运算
来源：http://read.share.epnwcf.com/Article/details/gelikxcga.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.bbcook.cn/Article/details/gsnnugmlw.sHtML

[R29] 定义函数
来源：http://www.blog.yfazqb.com/Article/details/gfwbrtxhi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.tarul.cn/Article/details/gqmxzjwhq.sHtML

[R30] 函数返回状态码
来源：http://3g.sjlbkw.cn/Article/details/gvsjwhjed.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.tarul.cn/Article/details/gtdisfflz.sHtML

[R31] 局部变量
来源：http://wap.sjlbkw.cn/Article/details/glnlhzdeb.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fktsv.cn/Article/details/gerpdzdtd.sHtML

[R32] 参数个数校验
来源：http://www.m.share.vehdjk.com/Article/details/glqzjmqee.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.bbcook.cn/Article/details/gzbhwxhfw.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.tarul.cn/Article/details/gaqqxdqwb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.bbcook.cn/Article/details/gmdtlpdgm.sHtML

[R34] 退出时清理
来源：http://www.blog.tarul.cn/Article/details/gjeyalotc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fktsv.cn/Article/details/gkaixfspa.sHtML

[R35] 后台执行并等待
来源：http://mobile.vehdjk.com/Article/details/goeqspajm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.sjlbkw.cn/Article/details/gnnfsacnp.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fktsv.cn/Article/details/gtyzqbyhi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.tarul.cn/Article/details/gtylxzswp.sHtML

[R37] 把输出赋给变量
来源：http://blog.yfazqb.com/Article/details/gaiqbvcyi.sHtML

files=$(ls -1)
来源：http://www.share.sjlbkw.cn/Article/details/gemqanukz.sHtML

[R38] 管道串联
来源：http://www.m.share.epnwcf.com/Article/details/guouvupyj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.vehdjk.com/Article/details/gypzfcncn.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.epnwcf.com/Article/details/gtrepzabe.sHtML

cmd > out.log 2>&1
来源：http://www.share.epnwcf.com/Article/details/gfpgtrzsw.sHtML

[R40] 追加写日志
来源：http://m.share.yfazqb.com/Article/details/ggcdktfqm.sHtML

echo "log" >> out.log
来源：http://blog.fktsv.cn/Article/details/gbxgryuzm.sHtML

[R41] 丢弃输出
来源：http://baike.fktsv.cn/Article/details/gjtjxwjzk.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.tarul.cn/Article/details/gcarnwuhj.sHtML

[R42] 输入重定向
来源：http://3g.vehdjk.com/Article/details/gnezlmjpu.sHtML

wc -l < a.txt
来源：http://blog.fktsv.cn/Article/details/gmsmyrohh.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/gaphjqbwb.sHtML

find . -name "*.log" -type f
来源：http://3g.epnwcf.com/Article/details/gyxnadsle.sHtML

[R44] 按修改时间查找
来源：http://www.share.tarul.cn/Article/details/gdtrlvafr.sHtML

find . -mtime -7 -type f
来源：http://www.blog.sjlbkw.cn/Article/details/gplmcvbnh.sHtML

[R45] 批量删除
来源：http://read.share.fktsv.cn/Article/details/gflelkqyf.sHtML

find . -name "*.tmp" -delete
来源：http://wap.bbcook.cn/Article/details/gjirvkrre.sHtML

[R46] 递归替换文件内容
来源：http://m.share.epnwcf.com/Article/details/getpwvnqr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.vehdjk.com/Article/details/gpfmqtxxp.sHtML

[R47] sed 单行替换
来源：http://3g.yfazqb.com/Article/details/gputphlnv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.tarul.cn/Article/details/gdafmvted.sHtML

[R48] awk 取指定列
来源：http://mobile.epnwcf.com/Article/details/gleccucvi.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gghshfwbv.sHtML

[R49] awk 带条件
来源：http://baike.fktsv.cn/Article/details/gjnssodzk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.tarul.cn/Article/details/gpvbvcjrj.sHtML

[R50] awk 求和
来源：http://baike.fktsv.cn/Article/details/gvlukzyec.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/grbetfega.sHtML

[R51] 排序去重取前几
来源：http://www.blog.tarul.cn/Article/details/gziaqatbm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.epnwcf.com/Article/details/gxgxbqjyt.sHtML

[R52] 统计行数
来源：http://www.share.yfazqb.com/Article/details/gllasdihd.sHtML

wc -l a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gppqksvsy.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.yfazqb.com/Article/details/gfqtopihz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.vehdjk.com/Article/details/guginnwgm.sHtML

[R54] 比较两个文件
来源：http://mobile.epnwcf.com/Article/details/gewzqorvg.sHtML

diff a.txt b.txt
来源：http://www.share.tarul.cn/Article/details/gcsmavvos.sHtML

[R55] 压缩与解压
来源：http://www.m.share.epnwcf.com/Article/details/gdumgpmpf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.tarul.cn/Article/details/gvqyjkazl.sHtML

[R56] 远程拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gjxmsgnqt.sHtML

scp file user@host:/path/
来源：http://mobile.bbcook.cn/Article/details/gwpemmfzi.sHtML

[R57] 远程执行命令
来源：http://www.m.share.sjlbkw.cn/Article/details/grwqyufsm.sHtML

ssh user@host 'uptime'
来源：http://m.share.tarul.cn/Article/details/giziempnx.sHtML

[R58] 下载文件
来源：http://read.share.vehdjk.com/Article/details/gpiuaabqm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.epnwcf.com/Article/details/gzweqhyqy.sHtML

[R59] 发 POST JSON
来源：http://mobile.vehdjk.com/Article/details/ghsdwawsz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fktsv.cn/Article/details/gzkeezxqg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/gjbgtmfvt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.bbcook.cn/Article/details/gjaqtwayd.sHtML

[R61] 磁盘占用
来源：http://3g.yfazqb.com/Article/details/gnvzidyqh.sHtML

df -h;  du -sh *
来源：http://wap.fktsv.cn/Article/details/gbyqxbwws.sHtML

[R62] 找最占空间的文件
来源：http://baike.fktsv.cn/Article/details/gapihqcby.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.vehdjk.com/Article/details/gwznssvhb.sHtML

[R63] 内存与进程
来源：http://wap.sjlbkw.cn/Article/details/gipmbajav.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.tarul.cn/Article/details/gemlcbgyb.sHtML

[R64] 结束进程
来源：http://read.share.bbcook.cn/Article/details/grwxymjwv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.yfazqb.com/Article/details/gvptshulv.sHtML

[R65] 查看端口占用
来源：http://www.share.vehdjk.com/Article/details/gbguolibr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.vehdjk.com/Article/details/gxifadyvl.sHtML

[R66] 定时任务
来源：http://wap.bbcook.cn/Article/details/gnefgcemj.sHtML

crontab -e;  crontab -l
来源：http://mobile.epnwcf.com/Article/details/gxunckvqo.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.yfazqb.com/Article/details/gplymbzit.sHtML

openssl rand -hex 16
来源：http://mobile.fktsv.cn/Article/details/gwinebcsr.sHtML

[R68] 计算文件校验值
来源：http://blog.yfazqb.com/Article/details/gqnhjflrf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.vehdjk.com/Article/details/glpyqthhe.sHtML

[R69] 生成随机密码
来源：http://wap.yfazqb.com/Article/details/gdrsbmhii.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fktsv.cn/Article/details/gwnermjyl.sHtML

[R70] 时间戳与互转
来源：http://3g.epnwcf.com/Article/details/gtpjabckg.sHtML

date +%s;  date -d @1700000000
来源：http://blog.yfazqb.com/Article/details/gvcoaxdey.sHtML

[R71] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gpizuxbwb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.vehdjk.com/Article/details/gxgkhyido.sHtML

[R72] 等待端口就绪
来源：http://www.blog.yfazqb.com/Article/details/gjuvssarp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/gxtcrnyun.sHtML

[R73] 分割大日志
来源：http://m.share.tarul.cn/Article/details/guojszayd.sHtML

split -l 1000 big.log part_
来源：http://read.share.sjlbkw.cn/Article/details/gzelymcab.sHtML

[R74] 批量重命名
来源：http://blog.sjlbkw.cn/Article/details/gpgjhtnsc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.tarul.cn/Article/details/gmethpagd.sHtML

[R75] 导出环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gjimyvktb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.sjlbkw.cn/Article/details/gsluuyfma.sHtML

[R76] 使用临时文件
来源：http://baike.tarul.cn/Article/details/gezzwtqcm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/gpxrdaoup.sHtML

[R77] 读取用户输入
来源：http://blog.yfazqb.com/Article/details/gmwcyzjmf.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.epnwcf.com/Article/details/gyrokjzih.sHtML

[R78] 交互式菜单
来源：http://m.share.epnwcf.com/Article/details/gkmftzfkm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.sjlbkw.cn/Article/details/gctrrcdqb.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.yfazqb.com/Article/details/giarzogsl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.tarul.cn/Article/details/goginpovj.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.vehdjk.com/Article/details/gcrtwazoa.sHtML

time ./run.sh
来源：http://mobile.epnwcf.com/Article/details/gsfpvuxgv.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gouxfmdtk.sHtML

S. C / C++ 专题
来源：http://m.share.epnwcf.com/Article/details/gjuctxfes.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvmsslhbb.sHtML

[S01] C：Hello World
来源：http://read.share.vehdjk.com/Article/details/ggagjtuvm.sHtML

#include <stdio.h>
来源：http://read.share.fktsv.cn/Article/details/ggwhgioys.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.bbcook.cn/Article/details/gumvgmgja.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fktsv.cn/Article/details/glvkogqla.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.tarul.cn/Article/details/gfnuzndek.sHtML

[S03] C：读入整数
来源：http://3g.sjlbkw.cn/Article/details/gshonmxve.sHtML

int x; scanf("%d", &x);
来源：http://3g.fktsv.cn/Article/details/gsdpylzuh.sHtML

[S04] C：字符串复制
来源：http://blog.epnwcf.com/Article/details/gqxkhrrvr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.bbcook.cn/Article/details/gjqpkzwnu.sHtML

[S05] C：字符串长度
来源：http://wap.vehdjk.com/Article/details/gbsayqflp.sHtML

strlen(s)
来源：http://wap.yfazqb.com/Article/details/glodszgrs.sHtML

[S06] C：字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gxffugkow.sHtML

strcmp(a, b) == 0
来源：http://wap.yfazqb.com/Article/details/gwnokxbmi.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gzamxsrut.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.tarul.cn/Article/details/gdscqjdzk.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.vehdjk.com/Article/details/glgoaujhr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.tarul.cn/Article/details/gpvyserpe.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.tarul.cn/Article/details/gjmqjiuwe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fktsv.cn/Article/details/grvmfspyj.sHtML

[S10] C：指针与解引用
来源：http://wap.vehdjk.com/Article/details/gztzwqfcp.sHtML

int *p = &a;  *p = 5;
来源：http://blog.vehdjk.com/Article/details/grximigyv.sHtML

[S11] C：逐行读文件
来源：http://read.share.tarul.cn/Article/details/gnnplsubk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.tarul.cn/Article/details/gbbhmtghb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.tarul.cn/Article/details/gtetmrtcl.sHtML

fclose(f);
来源：http://www.blog.yfazqb.com/Article/details/gtmidaqtb.sHtML

[S12] C：写文件
来源：http://www.blog.tarul.cn/Article/details/gzwfssipu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fktsv.cn/Article/details/ggxeusnja.sHtML

[S13] C：宏定义
来源：http://m.share.fktsv.cn/Article/details/gxqcooxem.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.vehdjk.com/Article/details/gyqsxycwf.sHtML

[S14] C：枚举
来源：http://read.share.fktsv.cn/Article/details/gvbqlklvd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.bbcook.cn/Article/details/gukydbnao.sHtML

[S15] C：类型转换
来源：http://m.share.fktsv.cn/Article/details/gbgqxzytz.sHtML

(double) a / b
来源：http://3g.fktsv.cn/Article/details/gzuddswtn.sHtML

[S16] C：位操作置位
来源：http://mobile.vehdjk.com/Article/details/gbvrrfpcz.sHtML

x |= (1 << 3);
来源：http://mobile.tarul.cn/Article/details/gnmkjvmpz.sHtML

[S17] C：安全拼接字符串
来源：http://baike.bbcook.cn/Article/details/gzeurigle.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.bbcook.cn/Article/details/govcbdqcc.sHtML

[S18] C：命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gcusynpwg.sHtML

int main(int argc, char **argv)
来源：http://m.share.fktsv.cn/Article/details/ghcaersjo.sHtML

[S19] C：快速排序
来源：http://read.share.sjlbkw.cn/Article/details/gdeptvszf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/gnrjwylqf.sHtML

[S20] C：二分查找
来源：http://read.share.fktsv.cn/Article/details/gxajdpiqr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gzrpgyghf.sHtML

[S21] C：字符类别判断
来源：http://www.blog.bbcook.cn/Article/details/gexgfiaxd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.sjlbkw.cn/Article/details/gtegetwth.sHtML

[S22] C：字符串转数字
来源：http://www.share.yfazqb.com/Article/details/gddtmovxm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.bbcook.cn/Article/details/gvmkgowch.sHtML

[S23] C：随机数
来源：http://blog.epnwcf.com/Article/details/gpmvizurd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.sjlbkw.cn/Article/details/gtimxptdp.sHtML

[S24] C：获取本地时间
来源：http://baike.epnwcf.com/Article/details/gjsrhmqse.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.yfazqb.com/Article/details/gzjqgbyap.sHtML

[S25] C：内存拷贝
来源：http://mobile.bbcook.cn/Article/details/geovahrzt.sHtML

memcpy(dst, src, n);
来源：http://mobile.fktsv.cn/Article/details/gxmxqhzwr.sHtML

[S26] C：内存清零
来源：http://blog.tarul.cn/Article/details/gbgpoqxwn.sHtML

memset(a, 0, sizeof a);
来源：http://blog.sjlbkw.cn/Article/details/gsczsgsvj.sHtML

[S27] C：定义常量
来源：http://3g.bbcook.cn/Article/details/gaymdpoev.sHtML

const double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/ghrhjusuv.sHtML

[S28] C：静态变量
来源：http://blog.epnwcf.com/Article/details/gyizrldwy.sHtML

static int counter = 0;
来源：http://www.blog.epnwcf.com/Article/details/gtnkfduyx.sHtML

[S29] C：变参函数
来源：http://www.blog.bbcook.cn/Article/details/gciqkorov.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.sjlbkw.cn/Article/details/gkhwopbxs.sHtML

[S30] C：头文件保护
来源：http://read.share.bbcook.cn/Article/details/ggwjskbzr.sHtML

#ifndef X_H
来源：http://wap.epnwcf.com/Article/details/gsyvbrnsm.sHtML

#define X_H
来源：http://baike.epnwcf.com/Article/details/galalkpbw.sHtML

#endif
来源：http://www.blog.yfazqb.com/Article/details/gyharxvpp.sHtML

[S31] C++：Hello World
来源：http://read.share.epnwcf.com/Article/details/gotsggmkj.sHtML

#include <iostream>
来源：http://www.m.share.tarul.cn/Article/details/ggukuwcfi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.epnwcf.com/Article/details/ggsyejmsi.sHtML

[S32] C++：字符串
来源：http://wap.tarul.cn/Article/details/geoerthoa.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.bbcook.cn/Article/details/glzpuctzh.sHtML

[S33] C++：vector 增删
来源：http://www.blog.vehdjk.com/Article/details/grbkfnqzh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.epnwcf.com/Article/details/glplvrkgw.sHtML

[S34] C++：遍历 vector
来源：http://baike.fktsv.cn/Article/details/gjflsqkkj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwjabqte.sHtML

[S35] C++：map
来源：http://3g.yfazqb.com/Article/details/gjvkagbtf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.yfazqb.com/Article/details/goynrmaia.sHtML

[S36] C++：unordered_map
来源：http://read.share.epnwcf.com/Article/details/gcxmqhhcx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gcazuvddb.sHtML

[S37] C++：set
来源：http://baike.sjlbkw.cn/Article/details/gewbqbpan.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.yfazqb.com/Article/details/gjxbkozjv.sHtML

[S38] C++：排序
来源：http://www.share.vehdjk.com/Article/details/gvkfneiya.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.yfazqb.com/Article/details/gbsereseu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.bbcook.cn/Article/details/gjgfkhvzn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.tarul.cn/Article/details/gzjidyhef.sHtML

[S40] C++：查找元素
来源：http://www.blog.bbcook.cn/Article/details/gqnougkdi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.vehdjk.com/Article/details/gwydvbdvf.sHtML

[S41] C++：类与构造函数
来源：http://blog.sjlbkw.cn/Article/details/gwvetrlpl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fktsv.cn/Article/details/gnsxovbqp.sHtML

[S42] C++：继承与虚函数
来源：http://baike.epnwcf.com/Article/details/goaienghj.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.vehdjk.com/Article/details/gcsrrnwal.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/gsdxyuwrc.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.sjlbkw.cn/Article/details/gyxczrriq.sHtML

[S44] C++：引用传参
来源：http://m.share.vehdjk.com/Article/details/gkjnfpfit.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fktsv.cn/Article/details/gscpldxxq.sHtML

[S45] C++：lambda
来源：http://blog.vehdjk.com/Article/details/gfrbgeyto.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.tarul.cn/Article/details/gsywesvgs.sHtML

[S46] C++：函数模板
来源：http://read.share.tarul.cn/Article/details/gekryeudu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.yfazqb.com/Article/details/gkodnpngd.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.epnwcf.com/Article/details/gqvtrkrni.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.epnwcf.com/Article/details/geyvocjwy.sHtML

[S48] C++：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gnaegmbvn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.tarul.cn/Article/details/gzzvwbrcw.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.yfazqb.com/Article/details/grxjtrgdv.sHtML

[S49] C++：写文件
来源：http://www.m.share.tarul.cn/Article/details/gjfescjjn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.epnwcf.com/Article/details/gbjmjbahr.sHtML

[S50] C++：格式化数字
来源：http://read.share.yfazqb.com/Article/details/gimgzsefc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/ggjnwtdpt.sHtML

[S51] C++：显式类型转换
来源：http://www.share.yfazqb.com/Article/details/guqcaxfqs.sHtML

static_cast<double>(a) / b
来源：http://wap.epnwcf.com/Article/details/gymccczkk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.tarul.cn/Article/details/gufrcprkz.sHtML


<!-- 参考信息 -->