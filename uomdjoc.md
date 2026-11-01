代发 wailian999

[Q80] 字符串截取
来源：http://blog.vehdjk.com/Article/details/gvjhjokgv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gsqbabgru.sHtML

[Q81] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gflezihta.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gziyejzwc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.sjlbkw.cn/Article/details/garirpgot.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gueupcrdi.sHtML

[Q83] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gxbdbyjwj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gtaeqoics.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.yfazqb.com/Article/details/guvinbxay.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/gxwdtjexi.sHtML

[Q85] 数值取整
来源：http://www.blog.yfazqb.com/Article/details/gwhoaqoru.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.vehdjk.com/Article/details/ghdevyfew.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.tarul.cn/Article/details/ghfaypyqp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.tarul.cn/Article/details/goityvkuq.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.vehdjk.com/Article/details/gfwfxgkoc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.yfazqb.com/Article/details/gcinhzblx.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.vehdjk.com/Article/details/glmfxrcyq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.sjlbkw.cn/Article/details/glopxxjmm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/grebjeurz.sHtML

[Q89] 判断表是否存在
来源：http://blog.bbcook.cn/Article/details/guooxqveb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.epnwcf.com/Article/details/gklmpmjgv.sHtML

[Q90] 生成序号列
来源：http://www.blog.epnwcf.com/Article/details/glnwwxixj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.tarul.cn/Article/details/grbgfhzkm.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gvffzdlyn.sHtML

R. Bash 专题
来源：http://www.share.tarul.cn/Article/details/gkesxepdq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gcxqvlolv.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.vehdjk.com/Article/details/gpzossxme.sHtML

#!/usr/bin/env bash
来源：http://3g.tarul.cn/Article/details/gtirhubnp.sHtML

set -euo pipefail
来源：http://www.share.sjlbkw.cn/Article/details/gkixwkplj.sHtML

[R02] 变量赋值与使用
来源：http://baike.epnwcf.com/Article/details/gnnefswor.sHtML

name="Tom"; echo "$name"
来源：http://mobile.sjlbkw.cn/Article/details/gkhkolfav.sHtML

[R03] 只读变量
来源：http://www.m.share.epnwcf.com/Article/details/grcyeguea.sHtML

readonly PI=3.14
来源：http://blog.bbcook.cn/Article/details/gwnbmerej.sHtML

[R04] 位置参数
来源：http://www.blog.epnwcf.com/Article/details/gcujcxyac.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.epnwcf.com/Article/details/gtzwmqhkh.sHtML

[R05] 参数默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gyraytcqi.sHtML

name="${1:-default}"
来源：http://blog.fktsv.cn/Article/details/grigghuvy.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.tarul.cn/Article/details/gborontux.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.sjlbkw.cn/Article/details/gdkvctptp.sHtML

[R07] if 判断文件
来源：http://mobile.tarul.cn/Article/details/gciachkfb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.tarul.cn/Article/details/grfnmkcgp.sHtML

[R08] 数值比较
来源：http://read.share.fktsv.cn/Article/details/gmhihrgbf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.vehdjk.com/Article/details/gqaqqrjpn.sHtML

[R09] 字符串比较
来源：http://www.blog.epnwcf.com/Article/details/gungazlyr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gbflhryfn.sHtML

[R10] 正则匹配
来源：http://read.share.fktsv.cn/Article/details/girzsiecr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.epnwcf.com/Article/details/gohapskmm.sHtML

[R11] case 多分支
来源：http://www.share.bbcook.cn/Article/details/gcgjwxqlx.sHtML

case "$1" in
来源：http://blog.epnwcf.com/Article/details/goyrhhvdk.sHtML

start) echo "启动" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gcglumarl.sHtML

stop)  echo "停止" ;;
来源：http://mobile.bbcook.cn/Article/details/gbhcfdjtb.sHtML

*)     echo "未知命令" ;;
来源：http://wap.sjlbkw.cn/Article/details/gnrrqeaup.sHtML

esac
来源：http://m.share.epnwcf.com/Article/details/ghtgcuyov.sHtML

[R12] for 遍历文件
来源：http://wap.yfazqb.com/Article/details/gdiblkdgz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fktsv.cn/Article/details/gctbyylkc.sHtML

[R13] for 计数循环
来源：http://blog.vehdjk.com/Article/details/gbpclcypi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.sjlbkw.cn/Article/details/gkxtgmaxl.sHtML

[R14] C 风格 for
来源：http://mobile.bbcook.cn/Article/details/guedyqisc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fktsv.cn/Article/details/gbihpucpa.sHtML

[R15] while 逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gzoevtprg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fktsv.cn/Article/details/ggriedmpd.sHtML

[R16] until 等待条件
来源：http://mobile.bbcook.cn/Article/details/gdceleybf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/gvxbqklkt.sHtML

[R17] 数组定义与取值
来源：http://mobile.tarul.cn/Article/details/gxcjznjni.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.epnwcf.com/Article/details/ghegqfpax.sHtML

[R18] 遍历数组
来源：http://read.share.vehdjk.com/Article/details/gabjuipdk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fktsv.cn/Article/details/grajxxhei.sHtML

[R19] 数组长度
来源：http://m.share.yfazqb.com/Article/details/gmilxymwd.sHtML

echo "${#arr[@]}"
来源：http://baike.yfazqb.com/Article/details/ggjdpncaj.sHtML

[R20] 关联数组（字典）
来源：http://wap.bbcook.cn/Article/details/glvgigxkd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.epnwcf.com/Article/details/goykwtrdu.sHtML

[R21] 字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gcsgxvnsi.sHtML

echo "${#s}"
来源：http://mobile.tarul.cn/Article/details/gzvhfhztw.sHtML

[R22] 截取子串
来源：http://wap.yfazqb.com/Article/details/gaxgtmjpm.sHtML

echo "${s:0:5}"
来源：http://www.blog.bbcook.cn/Article/details/gpdkjicna.sHtML

[R23] 字符串替换
来源：http://blog.yfazqb.com/Article/details/gnribjpxc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.vehdjk.com/Article/details/gfuuyhnob.sHtML

[R24] 大小写转换
来源：http://blog.tarul.cn/Article/details/gejpwjpgv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.vehdjk.com/Article/details/guvggjktc.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.epnwcf.com/Article/details/gcxfxhcfh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.bbcook.cn/Article/details/gwuzqdgww.sHtML

[R26] 命令替换
来源：http://baike.tarul.cn/Article/details/gwzgrvnzb.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.epnwcf.com/Article/details/gxbmrkreg.sHtML

[R27] 算术展开
来源：http://www.m.share.vehdjk.com/Article/details/gakxexrwx.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fktsv.cn/Article/details/gkabskyco.sHtML

[R28] 浮点运算
来源：http://www.m.share.fktsv.cn/Article/details/gryoblciw.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fktsv.cn/Article/details/gbhwerxiw.sHtML

[R29] 定义函数
来源：http://3g.yfazqb.com/Article/details/gktmnloam.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fktsv.cn/Article/details/gzvzqqajf.sHtML

[R30] 函数返回状态码
来源：http://blog.fktsv.cn/Article/details/gwgjnqiji.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fktsv.cn/Article/details/glflmbypm.sHtML

[R31] 局部变量
来源：http://mobile.epnwcf.com/Article/details/gnacvmtjk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.yfazqb.com/Article/details/gdwbayxrv.sHtML

[R32] 参数个数校验
来源：http://read.share.sjlbkw.cn/Article/details/gmrcqwkun.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gxloskthx.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.bbcook.cn/Article/details/glmyyqzyz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.tarul.cn/Article/details/gvglpuhrv.sHtML

[R34] 退出时清理
来源：http://www.share.fktsv.cn/Article/details/gtgirhver.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/gibqcinly.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.bbcook.cn/Article/details/gmoqhyhkd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.sjlbkw.cn/Article/details/gqkvhmwhe.sHtML

[R36] 并发执行多个任务
来源：http://baike.tarul.cn/Article/details/gqpjucais.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.tarul.cn/Article/details/gqzowqkxj.sHtML

[R37] 把输出赋给变量
来源：http://wap.bbcook.cn/Article/details/gegxclxgp.sHtML

files=$(ls -1)
来源：http://baike.tarul.cn/Article/details/gflstftcx.sHtML

[R38] 管道串联
来源：http://mobile.yfazqb.com/Article/details/gsouezglk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.sjlbkw.cn/Article/details/gbfltvzml.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.yfazqb.com/Article/details/gpqwwxgfy.sHtML

cmd > out.log 2>&1
来源：http://wap.bbcook.cn/Article/details/gwuryxjgh.sHtML

[R40] 追加写日志
来源：http://m.share.vehdjk.com/Article/details/gygygxkga.sHtML

echo "log" >> out.log
来源：http://www.share.sjlbkw.cn/Article/details/gatmdwzwl.sHtML

[R41] 丢弃输出
来源：http://m.share.vehdjk.com/Article/details/gjhqxwrub.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gsfaouhhg.sHtML

[R42] 输入重定向
来源：http://mobile.fktsv.cn/Article/details/gwwhktrhm.sHtML

wc -l < a.txt
来源：http://3g.epnwcf.com/Article/details/gklwotxsw.sHtML

[R43] 按名字查找文件
来源：http://www.share.vehdjk.com/Article/details/gkejwistg.sHtML

find . -name "*.log" -type f
来源：http://www.share.bbcook.cn/Article/details/gduvixdej.sHtML

[R44] 按修改时间查找
来源：http://www.share.sjlbkw.cn/Article/details/glcftjkdq.sHtML

find . -mtime -7 -type f
来源：http://wap.epnwcf.com/Article/details/gywskfpxj.sHtML

[R45] 批量删除
来源：http://www.share.vehdjk.com/Article/details/glsrsctyp.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.bbcook.cn/Article/details/gjppwsqnq.sHtML

[R46] 递归替换文件内容
来源：http://mobile.tarul.cn/Article/details/gmiekknod.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.yfazqb.com/Article/details/gyjjhyifg.sHtML

[R47] sed 单行替换
来源：http://3g.vehdjk.com/Article/details/gopdlbahp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.bbcook.cn/Article/details/ggjwaswfe.sHtML

[R48] awk 取指定列
来源：http://m.share.tarul.cn/Article/details/gouxcfflc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gevnlruzr.sHtML

[R49] awk 带条件
来源：http://wap.yfazqb.com/Article/details/gtxobygfw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fktsv.cn/Article/details/gvbmqxdbm.sHtML

[R50] awk 求和
来源：http://www.m.share.bbcook.cn/Article/details/gukgikgvu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gnwadqcys.sHtML

[R51] 排序去重取前几
来源：http://www.blog.bbcook.cn/Article/details/giojotxpr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.sjlbkw.cn/Article/details/gnoalorbz.sHtML

[R52] 统计行数
来源：http://read.share.yfazqb.com/Article/details/gcytflmch.sHtML

wc -l a.txt
来源：http://wap.vehdjk.com/Article/details/gvnasjzla.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.bbcook.cn/Article/details/garvagmqe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.bbcook.cn/Article/details/gqdeluvbo.sHtML

[R54] 比较两个文件
来源：http://m.share.sjlbkw.cn/Article/details/gzwnbxvqd.sHtML

diff a.txt b.txt
来源：http://read.share.vehdjk.com/Article/details/glkkwqpze.sHtML

[R55] 压缩与解压
来源：http://read.share.epnwcf.com/Article/details/gxjnhpbke.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.vehdjk.com/Article/details/gboduhkto.sHtML

[R56] 远程拷贝
来源：http://www.blog.vehdjk.com/Article/details/gcctetkwx.sHtML

scp file user@host:/path/
来源：http://www.m.share.yfazqb.com/Article/details/gyisukcwa.sHtML

[R57] 远程执行命令
来源：http://www.share.sjlbkw.cn/Article/details/ggarmqpto.sHtML

ssh user@host 'uptime'
来源：http://mobile.tarul.cn/Article/details/gqjujpuhn.sHtML

[R58] 下载文件
来源：http://baike.epnwcf.com/Article/details/ggagemckt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.yfazqb.com/Article/details/gngteuzdv.sHtML

[R59] 发 POST JSON
来源：http://read.share.yfazqb.com/Article/details/glfyjoqea.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fktsv.cn/Article/details/gqaxdrlsf.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.yfazqb.com/Article/details/genjzmegv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fktsv.cn/Article/details/gmhyefpwu.sHtML

[R61] 磁盘占用
来源：http://www.m.share.yfazqb.com/Article/details/gobhbmdjl.sHtML

df -h;  du -sh *
来源：http://m.share.vehdjk.com/Article/details/gcvktrqvo.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fktsv.cn/Article/details/grwygbsiu.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.yfazqb.com/Article/details/gqjuttqvx.sHtML

[R63] 内存与进程
来源：http://www.blog.fktsv.cn/Article/details/gxkovuvot.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.vehdjk.com/Article/details/gbjzkdjbo.sHtML

[R64] 结束进程
来源：http://www.share.sjlbkw.cn/Article/details/gdjpjbmyp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.yfazqb.com/Article/details/gnwfxqnao.sHtML

[R65] 查看端口占用
来源：http://read.share.bbcook.cn/Article/details/gbxxcmrdy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.yfazqb.com/Article/details/gqwahplms.sHtML

[R66] 定时任务
来源：http://mobile.bbcook.cn/Article/details/ggdebyhyg.sHtML

crontab -e;  crontab -l
来源：http://read.share.tarul.cn/Article/details/gmnxmnljl.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.tarul.cn/Article/details/gzoixqmbd.sHtML

openssl rand -hex 16
来源：http://read.share.vehdjk.com/Article/details/gkpzvndob.sHtML

[R68] 计算文件校验值
来源：http://blog.bbcook.cn/Article/details/gtceqlrac.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.tarul.cn/Article/details/gbkwwerhx.sHtML

[R69] 生成随机密码
来源：http://mobile.yfazqb.com/Article/details/gxgrtbkwi.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.tarul.cn/Article/details/gcsdtnbaa.sHtML

[R70] 时间戳与互转
来源：http://read.share.epnwcf.com/Article/details/gaalmguvy.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.sjlbkw.cn/Article/details/guueqigfj.sHtML

[R71] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/ggkrduqye.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.epnwcf.com/Article/details/gdzwpkxml.sHtML

[R72] 等待端口就绪
来源：http://read.share.bbcook.cn/Article/details/gscdtkuqt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gozlxgstl.sHtML

[R73] 分割大日志
来源：http://www.blog.sjlbkw.cn/Article/details/gjtxthsbl.sHtML

split -l 1000 big.log part_
来源：http://baike.bbcook.cn/Article/details/gmdaxmtft.sHtML

[R74] 批量重命名
来源：http://read.share.tarul.cn/Article/details/gwtimlumv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvbnbbxp.sHtML

[R75] 导出环境变量
来源：http://blog.epnwcf.com/Article/details/gfeximabf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.sjlbkw.cn/Article/details/ggmfzjimq.sHtML

[R76] 使用临时文件
来源：http://www.blog.fktsv.cn/Article/details/gibestxbw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.tarul.cn/Article/details/gsncboxlp.sHtML

[R77] 读取用户输入
来源：http://3g.tarul.cn/Article/details/giaqkzrad.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.bbcook.cn/Article/details/gbawpjyib.sHtML

[R78] 交互式菜单
来源：http://wap.sjlbkw.cn/Article/details/gxcfvohuw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.tarul.cn/Article/details/gfahnqvii.sHtML

[R79] 解析命令行选项
来源：http://read.share.yfazqb.com/Article/details/gungrumfa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fktsv.cn/Article/details/gschhauys.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.sjlbkw.cn/Article/details/gpqufzpsn.sHtML

time ./run.sh
来源：http://www.share.sjlbkw.cn/Article/details/gkdkdstsf.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gwidwzrzk.sHtML

S. C / C++ 专题
来源：http://baike.epnwcf.com/Article/details/gccpxavwl.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/geqilgkfi.sHtML

[S01] C：Hello World
来源：http://blog.tarul.cn/Article/details/gitvrabvs.sHtML

#include <stdio.h>
来源：http://www.m.share.sjlbkw.cn/Article/details/guyjqatfy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.tarul.cn/Article/details/gxqctwpge.sHtML

[S02] C：变量与格式化输出
来源：http://wap.sjlbkw.cn/Article/details/gwihbcnsb.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.epnwcf.com/Article/details/gswqrwvwk.sHtML

[S03] C：读入整数
来源：http://mobile.sjlbkw.cn/Article/details/goofovkqw.sHtML

int x; scanf("%d", &x);
来源：http://baike.yfazqb.com/Article/details/gmtncxlfm.sHtML

[S04] C：字符串复制
来源：http://m.share.bbcook.cn/Article/details/geskvtvxx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.bbcook.cn/Article/details/gdgfzzzgp.sHtML

[S05] C：字符串长度
来源：http://read.share.fktsv.cn/Article/details/gnjjmsnqu.sHtML

strlen(s)
来源：http://read.share.bbcook.cn/Article/details/gjbhayrmn.sHtML

[S06] C：字符串比较
来源：http://www.share.yfazqb.com/Article/details/glbgzbamu.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgourfsx.sHtML

[S07] C：数组遍历求和
来源：http://blog.yfazqb.com/Article/details/gzxxbxfqq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.epnwcf.com/Article/details/gkidzppqv.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.epnwcf.com/Article/details/gpmqywwjm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.yfazqb.com/Article/details/gikstayna.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.epnwcf.com/Article/details/gylmquwjf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.bbcook.cn/Article/details/gxjkvxfct.sHtML

[S10] C：指针与解引用
来源：http://www.share.yfazqb.com/Article/details/gtijezyxo.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.sjlbkw.cn/Article/details/gaypypgwu.sHtML

[S11] C：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gxjjymppa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fktsv.cn/Article/details/ghajlgkol.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.tarul.cn/Article/details/gsflekdwp.sHtML

fclose(f);
来源：http://wap.yfazqb.com/Article/details/gwfjybdnp.sHtML

[S12] C：写文件
来源：http://read.share.bbcook.cn/Article/details/gbzoytaee.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fktsv.cn/Article/details/ghzculsbl.sHtML

[S13] C：宏定义
来源：http://www.blog.tarul.cn/Article/details/gkvotqkvu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.vehdjk.com/Article/details/gqmyourie.sHtML

[S14] C：枚举
来源：http://baike.fktsv.cn/Article/details/gzaljreqy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.epnwcf.com/Article/details/goniwpqcp.sHtML

[S15] C：类型转换
来源：http://m.share.epnwcf.com/Article/details/gymeamhyw.sHtML

(double) a / b
来源：http://baike.vehdjk.com/Article/details/gaqniygsu.sHtML

[S16] C：位操作置位
来源：http://blog.tarul.cn/Article/details/guqxxczdu.sHtML

x |= (1 << 3);
来源：http://www.share.tarul.cn/Article/details/gxrcantka.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/gjvxilacl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.vehdjk.com/Article/details/gmqhnnvzq.sHtML

[S18] C：命令行参数
来源：http://baike.sjlbkw.cn/Article/details/gtmsojrlm.sHtML

int main(int argc, char **argv)
来源：http://baike.yfazqb.com/Article/details/gtagdfoei.sHtML

[S19] C：快速排序
来源：http://m.share.vehdjk.com/Article/details/gsrpnkfga.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/gcvrmvdpf.sHtML

[S20] C：二分查找
来源：http://www.blog.yfazqb.com/Article/details/grkcyjuds.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/goqxrugoy.sHtML

[S21] C：字符类别判断
来源：http://m.share.bbcook.cn/Article/details/gijajkbra.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.bbcook.cn/Article/details/gblzlwqrc.sHtML

[S22] C：字符串转数字
来源：http://blog.yfazqb.com/Article/details/ghqiyghhq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.epnwcf.com/Article/details/gnpfnsgbz.sHtML

[S23] C：随机数
来源：http://mobile.yfazqb.com/Article/details/gylqjctby.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.tarul.cn/Article/details/gvxtjyuyg.sHtML

[S24] C：获取本地时间
来源：http://read.share.vehdjk.com/Article/details/glezitief.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fktsv.cn/Article/details/grkeaqdme.sHtML

[S25] C：内存拷贝
来源：http://mobile.bbcook.cn/Article/details/gnlfblrpn.sHtML

memcpy(dst, src, n);
来源：http://www.blog.bbcook.cn/Article/details/gguuvqxjb.sHtML

[S26] C：内存清零
来源：http://mobile.yfazqb.com/Article/details/gfbextsal.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.epnwcf.com/Article/details/gqawrgfsc.sHtML

[S27] C：定义常量
来源：http://blog.vehdjk.com/Article/details/gyfedaoyd.sHtML

const double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gehikdptu.sHtML

[S28] C：静态变量
来源：http://read.share.yfazqb.com/Article/details/ghxyjeqaj.sHtML

static int counter = 0;
来源：http://blog.yfazqb.com/Article/details/gauwmhnqa.sHtML

[S29] C：变参函数
来源：http://3g.bbcook.cn/Article/details/gtizscrkv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.bbcook.cn/Article/details/geezuujoz.sHtML

[S30] C：头文件保护
来源：http://www.blog.bbcook.cn/Article/details/gwnqefegc.sHtML

#ifndef X_H
来源：http://wap.tarul.cn/Article/details/gnfryoglg.sHtML

#define X_H
来源：http://wap.fktsv.cn/Article/details/gaeovlgjt.sHtML

#endif
来源：http://www.m.share.yfazqb.com/Article/details/gdeikbzgm.sHtML

[S31] C++：Hello World
来源：http://3g.fktsv.cn/Article/details/ggntffzdr.sHtML

#include <iostream>
来源：http://wap.yfazqb.com/Article/details/gcynwpvlb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.vehdjk.com/Article/details/grwraajtv.sHtML

[S32] C++：字符串
来源：http://www.blog.epnwcf.com/Article/details/gmaybskia.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.epnwcf.com/Article/details/gnxjoncgo.sHtML

[S33] C++：vector 增删
来源：http://blog.sjlbkw.cn/Article/details/gvlmbhvak.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.sjlbkw.cn/Article/details/gkfhksojs.sHtML

[S34] C++：遍历 vector
来源：http://blog.sjlbkw.cn/Article/details/guplefvwg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/gblhobtyh.sHtML

[S35] C++：map
来源：http://blog.tarul.cn/Article/details/gelvkskph.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gscalakmk.sHtML

[S36] C++：unordered_map
来源：http://wap.epnwcf.com/Article/details/ghichsots.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnwbhimv.sHtML

[S37] C++：set
来源：http://wap.epnwcf.com/Article/details/gfnmztesp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.tarul.cn/Article/details/gofeaikkr.sHtML

[S38] C++：排序
来源：http://www.blog.yfazqb.com/Article/details/glipqeduh.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.epnwcf.com/Article/details/gmaidkzzm.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.tarul.cn/Article/details/gfowookcd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.vehdjk.com/Article/details/gybcrbfwe.sHtML

[S40] C++：查找元素
来源：http://www.share.epnwcf.com/Article/details/gcqajpgcb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.yfazqb.com/Article/details/gzhozsuri.sHtML

[S41] C++：类与构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gnetulqfp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.bbcook.cn/Article/details/gmhgojlan.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.vehdjk.com/Article/details/gftaqvuik.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.epnwcf.com/Article/details/gzjqvgpwq.sHtML

[S43] C++：智能指针
来源：http://www.blog.bbcook.cn/Article/details/gadrdyiio.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.vehdjk.com/Article/details/gkomxhhui.sHtML

[S44] C++：引用传参
来源：http://mobile.fktsv.cn/Article/details/ggplpllng.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.tarul.cn/Article/details/geoludjzd.sHtML

[S45] C++：lambda
来源：http://baike.bbcook.cn/Article/details/goxenukno.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.epnwcf.com/Article/details/gaglghdya.sHtML

[S46] C++：函数模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvboolsw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fktsv.cn/Article/details/gilpydplu.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fktsv.cn/Article/details/ghjvazkco.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.tarul.cn/Article/details/goyftmfei.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/guzjxwyyl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.vehdjk.com/Article/details/gsgkvhqsv.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fktsv.cn/Article/details/gkekjmawz.sHtML

[S49] C++：写文件
来源：http://www.share.yfazqb.com/Article/details/gakkacsvj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.sjlbkw.cn/Article/details/gqtmdbcjz.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.bbcook.cn/Article/details/gvbwjztos.sHtML


<!-- 参考信息 -->