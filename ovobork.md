代发 wailian999

[Q84] 去除首尾空格
来源：http://www.share.vehdjk.com/Article/details/gacuyahhj.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gauqojjau.sHtML

[Q85] 数值取整
来源：http://m.share.epnwcf.com/Article/details/guaojtygr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.sjlbkw.cn/Article/details/gtfrpxpwk.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.vehdjk.com/Article/details/glbabrewk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.epnwcf.com/Article/details/gxuobxnuw.sHtML

[Q87] JSON 字段做条件
来源：http://blog.bbcook.cn/Article/details/gnupoceyd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.epnwcf.com/Article/details/gxlzbxebw.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.tarul.cn/Article/details/gfrkmaqag.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.epnwcf.com/Article/details/gpondeeuv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fktsv.cn/Article/details/glpwdpjpz.sHtML

[Q89] 判断表是否存在
来源：http://blog.epnwcf.com/Article/details/gpstjsije.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.vehdjk.com/Article/details/gwwqilzsy.sHtML

[Q90] 生成序号列
来源：http://baike.tarul.cn/Article/details/guujuowiw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.bbcook.cn/Article/details/geytnhnur.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gdjbazuyl.sHtML

R. Bash 专题
来源：http://read.share.vehdjk.com/Article/details/gctsulwzz.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gqawjfhtp.sHtML

[R01] shebang 与严格模式
来源：http://blog.epnwcf.com/Article/details/ggbzxjnxq.sHtML

#!/usr/bin/env bash
来源：http://baike.sjlbkw.cn/Article/details/giyjdsumk.sHtML

set -euo pipefail
来源：http://www.share.fktsv.cn/Article/details/govnxtbks.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.bbcook.cn/Article/details/gjmqfbctf.sHtML

name="Tom"; echo "$name"
来源：http://blog.vehdjk.com/Article/details/gyktkquar.sHtML

[R03] 只读变量
来源：http://m.share.bbcook.cn/Article/details/gvlymeajm.sHtML

readonly PI=3.14
来源：http://baike.bbcook.cn/Article/details/gwibxdalp.sHtML

[R04] 位置参数
来源：http://m.share.vehdjk.com/Article/details/gpzinieyf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.bbcook.cn/Article/details/gdstkiytm.sHtML

[R05] 参数默认值
来源：http://m.share.sjlbkw.cn/Article/details/gtubpbafz.sHtML

name="${1:-default}"
来源：http://www.share.fktsv.cn/Article/details/gcptjtkfb.sHtML

[R06] 判断命令是否存在
来源：http://wap.yfazqb.com/Article/details/gdcaqiccv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.yfazqb.com/Article/details/gmawcoipr.sHtML

[R07] if 判断文件
来源：http://3g.vehdjk.com/Article/details/gfxfrgpfs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gksrbidgr.sHtML

[R08] 数值比较
来源：http://baike.yfazqb.com/Article/details/gpbfcluvt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.vehdjk.com/Article/details/gddpkbqmt.sHtML

[R09] 字符串比较
来源：http://www.share.bbcook.cn/Article/details/gxvajqviy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fktsv.cn/Article/details/ggmpsxifd.sHtML

[R10] 正则匹配
来源：http://www.share.tarul.cn/Article/details/glloibfxc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.bbcook.cn/Article/details/gcdxkiukz.sHtML

[R11] case 多分支
来源：http://www.blog.sjlbkw.cn/Article/details/guwcpolln.sHtML

case "$1" in
来源：http://blog.fktsv.cn/Article/details/grdwwkbdv.sHtML

start) echo "启动" ;;
来源：http://www.blog.tarul.cn/Article/details/gsmdapvvn.sHtML

stop)  echo "停止" ;;
来源：http://3g.sjlbkw.cn/Article/details/gspqcwjzm.sHtML

*)     echo "未知命令" ;;
来源：http://baike.vehdjk.com/Article/details/gmnyerkxh.sHtML

esac
来源：http://baike.sjlbkw.cn/Article/details/gczchvrxl.sHtML

[R12] for 遍历文件
来源：http://m.share.epnwcf.com/Article/details/gcrmzlyac.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.bbcook.cn/Article/details/gbadqtcff.sHtML

[R13] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/gzwnztlss.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/gilnsxidk.sHtML

[R14] C 风格 for
来源：http://m.share.tarul.cn/Article/details/gqjntomsv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/gegrfdgjj.sHtML

[R15] while 逐行读文件
来源：http://wap.yfazqb.com/Article/details/gzeoswxkk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fktsv.cn/Article/details/gqbxinmqn.sHtML

[R16] until 等待条件
来源：http://www.blog.sjlbkw.cn/Article/details/ghwipvrfi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/gavbbodhw.sHtML

[R17] 数组定义与取值
来源：http://www.share.fktsv.cn/Article/details/gwslivdit.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fktsv.cn/Article/details/gdvletmia.sHtML

[R18] 遍历数组
来源：http://blog.sjlbkw.cn/Article/details/grvzdlxkk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.epnwcf.com/Article/details/gprrijlgz.sHtML

[R19] 数组长度
来源：http://read.share.fktsv.cn/Article/details/gzxeasvwp.sHtML

echo "${#arr[@]}"
来源：http://read.share.sjlbkw.cn/Article/details/gznxmklxu.sHtML

[R20] 关联数组（字典）
来源：http://wap.sjlbkw.cn/Article/details/gfapjrznx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.tarul.cn/Article/details/gfpqibihc.sHtML

[R21] 字符串长度
来源：http://www.blog.fktsv.cn/Article/details/gcngmpjwn.sHtML

echo "${#s}"
来源：http://baike.fktsv.cn/Article/details/gskxefaou.sHtML

[R22] 截取子串
来源：http://baike.fktsv.cn/Article/details/gqwpzdcox.sHtML

echo "${s:0:5}"
来源：http://blog.sjlbkw.cn/Article/details/gtexxopii.sHtML

[R23] 字符串替换
来源：http://wap.fktsv.cn/Article/details/grlnsbrsx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.bbcook.cn/Article/details/goaoulzwp.sHtML

[R24] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/gjoxmnlge.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.vehdjk.com/Article/details/glnxbizda.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.vehdjk.com/Article/details/glpfgqhzr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.vehdjk.com/Article/details/gsiazjqte.sHtML

[R26] 命令替换
来源：http://mobile.bbcook.cn/Article/details/grlcouuon.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.epnwcf.com/Article/details/gjhzjlkhd.sHtML

[R27] 算术展开
来源：http://blog.yfazqb.com/Article/details/govyvojpi.sHtML

echo $((1 + 2 * 3))
来源：http://blog.yfazqb.com/Article/details/gvjqbbbml.sHtML

[R28] 浮点运算
来源：http://read.share.epnwcf.com/Article/details/gndowhmke.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.tarul.cn/Article/details/gmmvjncdf.sHtML

[R29] 定义函数
来源：http://3g.fktsv.cn/Article/details/gonxkzpya.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.tarul.cn/Article/details/ggujgomnb.sHtML

[R30] 函数返回状态码
来源：http://mobile.tarul.cn/Article/details/goywxzjyh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fktsv.cn/Article/details/ggildcdzl.sHtML

[R31] 局部变量
来源：http://mobile.yfazqb.com/Article/details/gwbacfppv.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.tarul.cn/Article/details/gvdjptxod.sHtML

[R32] 参数个数校验
来源：http://mobile.sjlbkw.cn/Article/details/gfineworp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.vehdjk.com/Article/details/gmkcrtbck.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.epnwcf.com/Article/details/gkczglfjr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.sjlbkw.cn/Article/details/gzahwhvbd.sHtML

[R34] 退出时清理
来源：http://3g.fktsv.cn/Article/details/gieuhwmkw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.yfazqb.com/Article/details/gtaklsqna.sHtML

[R35] 后台执行并等待
来源：http://baike.bbcook.cn/Article/details/gvayyhnog.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fktsv.cn/Article/details/gjiipdnpf.sHtML

[R36] 并发执行多个任务
来源：http://m.share.sjlbkw.cn/Article/details/gwgxotxts.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.bbcook.cn/Article/details/gjrcmbggi.sHtML

[R37] 把输出赋给变量
来源：http://blog.sjlbkw.cn/Article/details/gdqixsnnf.sHtML

files=$(ls -1)
来源：http://blog.fktsv.cn/Article/details/gwxdqpncz.sHtML

[R38] 管道串联
来源：http://www.blog.tarul.cn/Article/details/gaakhmiao.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.epnwcf.com/Article/details/ghhcrgzeb.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.yfazqb.com/Article/details/grnuhksni.sHtML

cmd > out.log 2>&1
来源：http://blog.vehdjk.com/Article/details/glflmxsfm.sHtML

[R40] 追加写日志
来源：http://www.share.vehdjk.com/Article/details/gyqceqalq.sHtML

echo "log" >> out.log
来源：http://m.share.sjlbkw.cn/Article/details/giudkipis.sHtML

[R41] 丢弃输出
来源：http://m.share.yfazqb.com/Article/details/gztvvkkxa.sHtML

cmd >/dev/null 2>&1
来源：http://wap.tarul.cn/Article/details/gkltfeoye.sHtML

[R42] 输入重定向
来源：http://mobile.bbcook.cn/Article/details/gujjogpqz.sHtML

wc -l < a.txt
来源：http://blog.vehdjk.com/Article/details/graplikya.sHtML

[R43] 按名字查找文件
来源：http://3g.epnwcf.com/Article/details/gdazaoubn.sHtML

find . -name "*.log" -type f
来源：http://www.share.tarul.cn/Article/details/gjcekynfq.sHtML

[R44] 按修改时间查找
来源：http://www.share.sjlbkw.cn/Article/details/gzhvxlvek.sHtML

find . -mtime -7 -type f
来源：http://www.share.bbcook.cn/Article/details/gvqaymsau.sHtML

[R45] 批量删除
来源：http://m.share.vehdjk.com/Article/details/ggzuluwjm.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.tarul.cn/Article/details/gtbggejoe.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.tarul.cn/Article/details/gxyjnoylt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.sjlbkw.cn/Article/details/gqewyjizg.sHtML

[R47] sed 单行替换
来源：http://www.share.tarul.cn/Article/details/gcdrakzwt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gsaxhowvt.sHtML

[R48] awk 取指定列
来源：http://www.share.epnwcf.com/Article/details/gbvyexpjb.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.yfazqb.com/Article/details/gyserogar.sHtML

[R49] awk 带条件
来源：http://blog.fktsv.cn/Article/details/gdpdwfmsa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.vehdjk.com/Article/details/gzfbrdgkl.sHtML

[R50] awk 求和
来源：http://read.share.bbcook.cn/Article/details/glpixtsbn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.bbcook.cn/Article/details/gzhcqgjlr.sHtML

[R51] 排序去重取前几
来源：http://3g.vehdjk.com/Article/details/gcxuklknc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.epnwcf.com/Article/details/gywsqefsr.sHtML

[R52] 统计行数
来源：http://wap.vehdjk.com/Article/details/gsllutcyf.sHtML

wc -l a.txt
来源：http://3g.fktsv.cn/Article/details/gbpzzflrs.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.vehdjk.com/Article/details/geosrduqp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.tarul.cn/Article/details/gihnlihnd.sHtML

[R54] 比较两个文件
来源：http://www.m.share.epnwcf.com/Article/details/gqocasyte.sHtML

diff a.txt b.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gpabndabz.sHtML

[R55] 压缩与解压
来源：http://read.share.fktsv.cn/Article/details/gzsowocuq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.sjlbkw.cn/Article/details/gfvyivavl.sHtML

[R56] 远程拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gpwyuiiic.sHtML

scp file user@host:/path/
来源：http://baike.bbcook.cn/Article/details/gpyuduwbg.sHtML

[R57] 远程执行命令
来源：http://read.share.bbcook.cn/Article/details/gyczjxaqs.sHtML

ssh user@host 'uptime'
来源：http://read.share.vehdjk.com/Article/details/gvcycstux.sHtML

[R58] 下载文件
来源：http://blog.fktsv.cn/Article/details/gpmwtnoiy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.vehdjk.com/Article/details/gjtglfrkt.sHtML

[R59] 发 POST JSON
来源：http://www.share.sjlbkw.cn/Article/details/gbkaqeogf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.vehdjk.com/Article/details/gcitzlbxh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlcfurns.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.tarul.cn/Article/details/gjqzrzztq.sHtML

[R61] 磁盘占用
来源：http://wap.vehdjk.com/Article/details/gaftgxrqj.sHtML

df -h;  du -sh *
来源：http://m.share.yfazqb.com/Article/details/gnvewhnnh.sHtML

[R62] 找最占空间的文件
来源：http://blog.tarul.cn/Article/details/gsfigwcmc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.sjlbkw.cn/Article/details/gnaqyduoa.sHtML

[R63] 内存与进程
来源：http://read.share.sjlbkw.cn/Article/details/gacidygul.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.tarul.cn/Article/details/ggyqnhenh.sHtML

[R64] 结束进程
来源：http://www.m.share.yfazqb.com/Article/details/gvktlhjbi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.bbcook.cn/Article/details/gvjesbgaq.sHtML

[R65] 查看端口占用
来源：http://read.share.tarul.cn/Article/details/ghejkeqqp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.sjlbkw.cn/Article/details/gwmvluxrx.sHtML

[R66] 定时任务
来源：http://m.share.fktsv.cn/Article/details/geallzytw.sHtML

crontab -e;  crontab -l
来源：http://m.share.bbcook.cn/Article/details/gmzsrmikt.sHtML

[R67] 生成随机十六进制串
来源：http://blog.epnwcf.com/Article/details/gvegjvzpm.sHtML

openssl rand -hex 16
来源：http://wap.fktsv.cn/Article/details/gnwarsxxq.sHtML

[R68] 计算文件校验值
来源：http://www.share.tarul.cn/Article/details/gkxtnxawp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.epnwcf.com/Article/details/gvhvyuelo.sHtML

[R69] 生成随机密码
来源：http://baike.tarul.cn/Article/details/gcjsldgew.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.tarul.cn/Article/details/gbibfebhp.sHtML

[R70] 时间戳与互转
来源：http://m.share.tarul.cn/Article/details/gxwhznxpv.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fktsv.cn/Article/details/gdddlnvep.sHtML

[R71] 日期格式化
来源：http://blog.yfazqb.com/Article/details/gvgghbwof.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.yfazqb.com/Article/details/gietsaezn.sHtML

[R72] 等待端口就绪
来源：http://blog.fktsv.cn/Article/details/gmcaifudd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/gggsysnky.sHtML

[R73] 分割大日志
来源：http://3g.fktsv.cn/Article/details/gwprmzglg.sHtML

split -l 1000 big.log part_
来源：http://wap.yfazqb.com/Article/details/gvmqsawjw.sHtML

[R74] 批量重命名
来源：http://m.share.bbcook.cn/Article/details/glivlpesd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.bbcook.cn/Article/details/gjbvqntbz.sHtML

[R75] 导出环境变量
来源：http://www.blog.yfazqb.com/Article/details/gfomignom.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.epnwcf.com/Article/details/gxwwmycnf.sHtML

[R76] 使用临时文件
来源：http://blog.bbcook.cn/Article/details/gvrkhchsg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gknsggsxw.sHtML

[R77] 读取用户输入
来源：http://m.share.yfazqb.com/Article/details/gcacrnwfx.sHtML

read -rp "请输入: " ans
来源：http://www.share.fktsv.cn/Article/details/ghjycwezn.sHtML

[R78] 交互式菜单
来源：http://www.m.share.sjlbkw.cn/Article/details/gzypoljgl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.bbcook.cn/Article/details/gwbqrhofn.sHtML

[R79] 解析命令行选项
来源：http://mobile.tarul.cn/Article/details/gwfvrgliw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.yfazqb.com/Article/details/gfxbwezal.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fktsv.cn/Article/details/gleginbtz.sHtML

time ./run.sh
来源：http://www.m.share.vehdjk.com/Article/details/gulztmxld.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gmoatlicw.sHtML

S. C / C++ 专题
来源：http://m.share.tarul.cn/Article/details/gzxarzjyo.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gcvfnkzcl.sHtML

[S01] C：Hello World
来源：http://m.share.fktsv.cn/Article/details/gyzdnwmsf.sHtML

#include <stdio.h>
来源：http://www.blog.yfazqb.com/Article/details/gcloolqvh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.yfazqb.com/Article/details/gmkjkzret.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/gdnbfqsfd.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.vehdjk.com/Article/details/gmzdsueta.sHtML

[S03] C：读入整数
来源：http://3g.sjlbkw.cn/Article/details/gxtopablm.sHtML

int x; scanf("%d", &x);
来源：http://3g.sjlbkw.cn/Article/details/gpuyvpiku.sHtML

[S04] C：字符串复制
来源：http://mobile.sjlbkw.cn/Article/details/gumgxuuzb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.epnwcf.com/Article/details/gczcbceia.sHtML

[S05] C：字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gftcwuzvr.sHtML

strlen(s)
来源：http://blog.vehdjk.com/Article/details/gvdnzfweb.sHtML

[S06] C：字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/gmbizujqd.sHtML

strcmp(a, b) == 0
来源：http://www.share.tarul.cn/Article/details/gxemnxrjs.sHtML

[S07] C：数组遍历求和
来源：http://www.share.tarul.cn/Article/details/gguuumlmh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.vehdjk.com/Article/details/gdmthflyw.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.bbcook.cn/Article/details/gptskapid.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.vehdjk.com/Article/details/gvwopbpws.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.sjlbkw.cn/Article/details/gdzbknjba.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.bbcook.cn/Article/details/gqifxehug.sHtML

[S10] C：指针与解引用
来源：http://mobile.epnwcf.com/Article/details/gvcjbgltl.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.vehdjk.com/Article/details/gcnlkmxaf.sHtML

[S11] C：逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gybfxogtr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.tarul.cn/Article/details/gezsxwooy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fktsv.cn/Article/details/gxuxtkifd.sHtML

fclose(f);
来源：http://m.share.fktsv.cn/Article/details/ganrrhksu.sHtML

[S12] C：写文件
来源：http://wap.vehdjk.com/Article/details/glgcclybq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.bbcook.cn/Article/details/gqkwsuyon.sHtML

[S13] C：宏定义
来源：http://wap.epnwcf.com/Article/details/ggumwbisn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.yfazqb.com/Article/details/gilitnljs.sHtML

[S14] C：枚举
来源：http://www.blog.vehdjk.com/Article/details/ggwkaaxcy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.epnwcf.com/Article/details/gmyhmxhop.sHtML

[S15] C：类型转换
来源：http://www.m.share.tarul.cn/Article/details/gfsvkocjs.sHtML

(double) a / b
来源：http://read.share.vehdjk.com/Article/details/gtqugtzxz.sHtML

[S16] C：位操作置位
来源：http://wap.tarul.cn/Article/details/gwqheyndj.sHtML

x |= (1 << 3);
来源：http://mobile.fktsv.cn/Article/details/gozgbbbhs.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrxinboa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.vehdjk.com/Article/details/gmtflpjch.sHtML

[S18] C：命令行参数
来源：http://www.m.share.vehdjk.com/Article/details/gsxldhcjq.sHtML

int main(int argc, char **argv)
来源：http://read.share.vehdjk.com/Article/details/gqhfuqbjh.sHtML

[S19] C：快速排序
来源：http://www.m.share.fktsv.cn/Article/details/gglwodcsz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.epnwcf.com/Article/details/gashkinai.sHtML

[S20] C：二分查找
来源：http://www.blog.sjlbkw.cn/Article/details/gxahxauwq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/gljtemmbv.sHtML

[S21] C：字符类别判断
来源：http://baike.epnwcf.com/Article/details/gfzjuvjma.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.yfazqb.com/Article/details/gcfsiybfo.sHtML

[S22] C：字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gzindekqg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.sjlbkw.cn/Article/details/genddnxjg.sHtML

[S23] C：随机数
来源：http://baike.sjlbkw.cn/Article/details/geqclcqch.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.epnwcf.com/Article/details/gtyuyqrgl.sHtML

[S24] C：获取本地时间
来源：http://m.share.bbcook.cn/Article/details/gjzdsaxjn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.vehdjk.com/Article/details/gggxrvyyf.sHtML

[S25] C：内存拷贝
来源：http://blog.sjlbkw.cn/Article/details/ggduzccvv.sHtML

memcpy(dst, src, n);
来源：http://3g.yfazqb.com/Article/details/gitqmrxjy.sHtML

[S26] C：内存清零
来源：http://m.share.bbcook.cn/Article/details/gyqzxyvym.sHtML

memset(a, 0, sizeof a);
来源：http://wap.tarul.cn/Article/details/gzvbdnmjl.sHtML

[S27] C：定义常量
来源：http://read.share.sjlbkw.cn/Article/details/gyncejsco.sHtML

const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gamfkposh.sHtML

[S28] C：静态变量
来源：http://m.share.sjlbkw.cn/Article/details/gbvdbgffb.sHtML

static int counter = 0;
来源：http://m.share.sjlbkw.cn/Article/details/gnkmlfqje.sHtML

[S29] C：变参函数
来源：http://www.blog.epnwcf.com/Article/details/gxqbrmslb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.yfazqb.com/Article/details/gdmcqxmxq.sHtML

[S30] C：头文件保护
来源：http://m.share.sjlbkw.cn/Article/details/gahxlzyut.sHtML

#ifndef X_H
来源：http://www.m.share.epnwcf.com/Article/details/giljsbmpf.sHtML

#define X_H
来源：http://read.share.yfazqb.com/Article/details/gweatvvam.sHtML

#endif
来源：http://www.blog.yfazqb.com/Article/details/gyzrxdfqb.sHtML

[S31] C++：Hello World
来源：http://baike.bbcook.cn/Article/details/ggertigrx.sHtML

#include <iostream>
来源：http://baike.tarul.cn/Article/details/gosspwvnd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.tarul.cn/Article/details/gnxcpawfr.sHtML

[S32] C++：字符串
来源：http://wap.sjlbkw.cn/Article/details/gmdltppgd.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.tarul.cn/Article/details/ggbntzhof.sHtML

[S33] C++：vector 增删
来源：http://mobile.fktsv.cn/Article/details/gzrncndyg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.sjlbkw.cn/Article/details/gdvidwxsk.sHtML

[S34] C++：遍历 vector
来源：http://blog.sjlbkw.cn/Article/details/gwumlbvul.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.yfazqb.com/Article/details/gtmbibcct.sHtML

[S35] C++：map
来源：http://mobile.tarul.cn/Article/details/gypkkpfqi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gfwnqxfux.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.yfazqb.com/Article/details/gibcwpsvq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gonrqcuqe.sHtML

[S37] C++：set
来源：http://m.share.tarul.cn/Article/details/glwaocbrb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.bbcook.cn/Article/details/grsngfhyh.sHtML

[S38] C++：排序
来源：http://wap.bbcook.cn/Article/details/gdmhomzrc.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.tarul.cn/Article/details/giaqckqpj.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.sjlbkw.cn/Article/details/gjhusqnfm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.bbcook.cn/Article/details/gmosarsqs.sHtML

[S40] C++：查找元素
来源：http://www.share.vehdjk.com/Article/details/giwwnnuig.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.vehdjk.com/Article/details/ghlordlmy.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.tarul.cn/Article/details/gtxfwgrex.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.vehdjk.com/Article/details/gkivzytwc.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.sjlbkw.cn/Article/details/glyewvoma.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrybomhb.sHtML

[S43] C++：智能指针
来源：http://mobile.sjlbkw.cn/Article/details/gaicyohgv.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.vehdjk.com/Article/details/gymjqswom.sHtML

[S44] C++：引用传参
来源：http://read.share.tarul.cn/Article/details/gigclchiq.sHtML

void inc(int &x) { ++x; }
来源：http://wap.vehdjk.com/Article/details/gtkdgmcug.sHtML

[S45] C++：lambda
来源：http://www.share.fktsv.cn/Article/details/gudoyxjbp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.sjlbkw.cn/Article/details/gjvgbdizv.sHtML

[S46] C++：函数模板
来源：http://3g.tarul.cn/Article/details/gvhujuypt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.tarul.cn/Article/details/ghewoaeew.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.tarul.cn/Article/details/gnmothsqj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.bbcook.cn/Article/details/ggvfpwwww.sHtML

[S48] C++：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gwczynkbr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.epnwcf.com/Article/details/gponoslfl.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.sjlbkw.cn/Article/details/gxejmzzmp.sHtML

[S49] C++：写文件
来源：http://blog.bbcook.cn/Article/details/gqhkmbjyx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fktsv.cn/Article/details/gjnpfsvzm.sHtML

[S50] C++：格式化数字
来源：http://blog.epnwcf.com/Article/details/gacvwwqgv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gskrwkzkg.sHtML

[S51] C++：显式类型转换
来源：http://blog.vehdjk.com/Article/details/grcicxpjx.sHtML

static_cast<double>(a) / b
来源：http://mobile.tarul.cn/Article/details/gkrxogyct.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.bbcook.cn/Article/details/gvxeczwtv.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.bbcook.cn/Article/details/gaevqwlvt.sHtML

[S53] C++：移动语义
来源：http://m.share.bbcook.cn/Article/details/geqweoeom.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.yfazqb.com/Article/details/grkxodhgq.sHtML

[S54] C++：异常处理
来源：http://www.share.epnwcf.com/Article/details/goacexwsg.sHtML


<!-- 参考信息 -->