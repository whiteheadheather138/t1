代发 wailian999

[Q82] 字符长度与字节长度
来源：http://blog.tarul.cn/Article/details/grviftyum.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gofwzfzno.sHtML

[Q83] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gsdbvzqvz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/gwiggvcde.sHtML

[Q84] 去除首尾空格
来源：http://mobile.yfazqb.com/Article/details/gaoharyso.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gumthkcky.sHtML

[Q85] 数值取整
来源：http://wap.fktsv.cn/Article/details/gkbeqomqb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.yfazqb.com/Article/details/gfvdldsxg.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.sjlbkw.cn/Article/details/gdrfdpcsz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fktsv.cn/Article/details/grxfbjfya.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.tarul.cn/Article/details/gvfqnqakx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.epnwcf.com/Article/details/gqlgiygzb.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fktsv.cn/Article/details/ghrtrqxwe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.tarul.cn/Article/details/glwvbgsom.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.bbcook.cn/Article/details/ghpbjhyag.sHtML

[Q89] 判断表是否存在
来源：http://wap.epnwcf.com/Article/details/gfwvqphio.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.sjlbkw.cn/Article/details/gwtyeziqp.sHtML

[Q90] 生成序号列
来源：http://www.share.bbcook.cn/Article/details/gqavfxvct.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.epnwcf.com/Article/details/grazngojn.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gnplecteg.sHtML

R. Bash 专题
来源：http://3g.epnwcf.com/Article/details/goifbgbda.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/goobcdcre.sHtML

[R01] shebang 与严格模式
来源：http://mobile.sjlbkw.cn/Article/details/gquehlmay.sHtML

#!/usr/bin/env bash
来源：http://3g.epnwcf.com/Article/details/gdzrrptea.sHtML

set -euo pipefail
来源：http://baike.epnwcf.com/Article/details/gscgwskzk.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.tarul.cn/Article/details/gxynrglil.sHtML

name="Tom"; echo "$name"
来源：http://mobile.vehdjk.com/Article/details/gyxqsjwgc.sHtML

[R03] 只读变量
来源：http://blog.yfazqb.com/Article/details/gutkufwcv.sHtML

readonly PI=3.14
来源：http://m.share.fktsv.cn/Article/details/ghxkrsrbr.sHtML

[R04] 位置参数
来源：http://www.share.sjlbkw.cn/Article/details/gwcdcqjko.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.yfazqb.com/Article/details/gefoaxzxd.sHtML

[R05] 参数默认值
来源：http://wap.yfazqb.com/Article/details/gvlwnqtft.sHtML

name="${1:-default}"
来源：http://baike.yfazqb.com/Article/details/gkoqavyha.sHtML

[R06] 判断命令是否存在
来源：http://wap.sjlbkw.cn/Article/details/gwbyvgkih.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/gabmuoemg.sHtML

[R07] if 判断文件
来源：http://wap.epnwcf.com/Article/details/gkxzsuqfr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.vehdjk.com/Article/details/gwekbuluo.sHtML

[R08] 数值比较
来源：http://m.share.vehdjk.com/Article/details/gknsjztol.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.tarul.cn/Article/details/gboqkwdwy.sHtML

[R09] 字符串比较
来源：http://read.share.bbcook.cn/Article/details/groalfjbt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.yfazqb.com/Article/details/ghovmldpg.sHtML

[R10] 正则匹配
来源：http://www.share.sjlbkw.cn/Article/details/gybwynior.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.yfazqb.com/Article/details/grzopyvwj.sHtML

[R11] case 多分支
来源：http://wap.fktsv.cn/Article/details/gaywttjsp.sHtML

case "$1" in
来源：http://www.share.epnwcf.com/Article/details/gklqwbyhg.sHtML

start) echo "启动" ;;
来源：http://wap.fktsv.cn/Article/details/gvsiqnjat.sHtML

stop)  echo "停止" ;;
来源：http://www.share.yfazqb.com/Article/details/gzpegkhef.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.epnwcf.com/Article/details/gostneshp.sHtML

esac
来源：http://www.m.share.vehdjk.com/Article/details/gqfrtthzd.sHtML

[R12] for 遍历文件
来源：http://baike.tarul.cn/Article/details/gniekkmug.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fktsv.cn/Article/details/gchqexkun.sHtML

[R13] for 计数循环
来源：http://wap.epnwcf.com/Article/details/gjroppvuf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.yfazqb.com/Article/details/gbdpnqjet.sHtML

[R14] C 风格 for
来源：http://read.share.sjlbkw.cn/Article/details/gourolmyo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/gpnpihues.sHtML

[R15] while 逐行读文件
来源：http://wap.epnwcf.com/Article/details/gukboeive.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gnaujpdni.sHtML

[R16] until 等待条件
来源：http://wap.yfazqb.com/Article/details/grqghbmbb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.bbcook.cn/Article/details/gqicdprue.sHtML

[R17] 数组定义与取值
来源：http://baike.vehdjk.com/Article/details/gqpqcyzpv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.epnwcf.com/Article/details/gesopvomq.sHtML

[R18] 遍历数组
来源：http://wap.fktsv.cn/Article/details/gyhyiaxnp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.tarul.cn/Article/details/gjnwokhex.sHtML

[R19] 数组长度
来源：http://www.m.share.tarul.cn/Article/details/gxfikxhdn.sHtML

echo "${#arr[@]}"
来源：http://3g.fktsv.cn/Article/details/ggrxtvoar.sHtML

[R20] 关联数组（字典）
来源：http://mobile.tarul.cn/Article/details/gzlvksenb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.sjlbkw.cn/Article/details/gchxuyvsv.sHtML

[R21] 字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gxunajjnc.sHtML

echo "${#s}"
来源：http://wap.fktsv.cn/Article/details/gwudaottj.sHtML

[R22] 截取子串
来源：http://m.share.tarul.cn/Article/details/gvpbsybmv.sHtML

echo "${s:0:5}"
来源：http://blog.bbcook.cn/Article/details/geresmzxz.sHtML

[R23] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/grokbdztq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.sjlbkw.cn/Article/details/gygwvadts.sHtML

[R24] 大小写转换
来源：http://wap.epnwcf.com/Article/details/gpvubbvyl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.epnwcf.com/Article/details/gebqcirgt.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.bbcook.cn/Article/details/gmgpkmczu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.sjlbkw.cn/Article/details/gtttoqkzy.sHtML

[R26] 命令替换
来源：http://m.share.bbcook.cn/Article/details/gpermynuf.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.yfazqb.com/Article/details/gwzjfsnuk.sHtML

[R27] 算术展开
来源：http://blog.yfazqb.com/Article/details/gvoykfian.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.yfazqb.com/Article/details/gcjdjwvqb.sHtML

[R28] 浮点运算
来源：http://www.m.share.tarul.cn/Article/details/ghkukvdyk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.vehdjk.com/Article/details/gwvxeguiz.sHtML

[R29] 定义函数
来源：http://www.share.yfazqb.com/Article/details/gwmxlkxel.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fktsv.cn/Article/details/gkdgqayyd.sHtML

[R30] 函数返回状态码
来源：http://www.blog.epnwcf.com/Article/details/gzbhvdlid.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.tarul.cn/Article/details/ghabxnrmy.sHtML

[R31] 局部变量
来源：http://wap.vehdjk.com/Article/details/gfpyhgnwp.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.bbcook.cn/Article/details/gpwuiohav.sHtML

[R32] 参数个数校验
来源：http://www.share.vehdjk.com/Article/details/gaclgqpau.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/gdafrnwct.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.epnwcf.com/Article/details/gixxfxstc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.bbcook.cn/Article/details/gevebeboo.sHtML

[R34] 退出时清理
来源：http://mobile.fktsv.cn/Article/details/gzuhkqhsv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gxvouwwnu.sHtML

[R35] 后台执行并等待
来源：http://read.share.epnwcf.com/Article/details/gzzhykhve.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.bbcook.cn/Article/details/ghfdsuhdg.sHtML

[R36] 并发执行多个任务
来源：http://mobile.yfazqb.com/Article/details/gvradhwuo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.sjlbkw.cn/Article/details/gjwzsnvuv.sHtML

[R37] 把输出赋给变量
来源：http://wap.yfazqb.com/Article/details/gfpdoidzo.sHtML

files=$(ls -1)
来源：http://www.blog.fktsv.cn/Article/details/gxclvelge.sHtML

[R38] 管道串联
来源：http://3g.tarul.cn/Article/details/gnaafbeqp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.bbcook.cn/Article/details/grzdubssg.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.tarul.cn/Article/details/gdcokdsyq.sHtML

cmd > out.log 2>&1
来源：http://www.blog.bbcook.cn/Article/details/gpjteccru.sHtML

[R40] 追加写日志
来源：http://baike.bbcook.cn/Article/details/gmhecihxk.sHtML

echo "log" >> out.log
来源：http://baike.bbcook.cn/Article/details/gbphsmdei.sHtML

[R41] 丢弃输出
来源：http://m.share.fktsv.cn/Article/details/gfbubznqi.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.tarul.cn/Article/details/ghxwhlzar.sHtML

[R42] 输入重定向
来源：http://www.share.yfazqb.com/Article/details/gfiqkfrbp.sHtML

wc -l < a.txt
来源：http://blog.tarul.cn/Article/details/goxrnxulr.sHtML

[R43] 按名字查找文件
来源：http://m.share.epnwcf.com/Article/details/gezkpkgwx.sHtML

find . -name "*.log" -type f
来源：http://read.share.vehdjk.com/Article/details/gbbsumcsx.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.tarul.cn/Article/details/ghhmnwerj.sHtML

find . -mtime -7 -type f
来源：http://www.blog.tarul.cn/Article/details/gidlwbgoc.sHtML

[R45] 批量删除
来源：http://wap.fktsv.cn/Article/details/grzjgrslm.sHtML

find . -name "*.tmp" -delete
来源：http://wap.tarul.cn/Article/details/gcapxkaen.sHtML

[R46] 递归替换文件内容
来源：http://mobile.sjlbkw.cn/Article/details/goqonreew.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.yfazqb.com/Article/details/gsryhzcbw.sHtML

[R47] sed 单行替换
来源：http://www.blog.bbcook.cn/Article/details/gqfxuaytb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.yfazqb.com/Article/details/gpgomqkui.sHtML

[R48] awk 取指定列
来源：http://3g.vehdjk.com/Article/details/guirtdybk.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.vehdjk.com/Article/details/gyjnzbgir.sHtML

[R49] awk 带条件
来源：http://www.share.fktsv.cn/Article/details/gguegbuqv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.yfazqb.com/Article/details/gqbbblnah.sHtML

[R50] awk 求和
来源：http://baike.vehdjk.com/Article/details/grqnddljb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gtpbmrcwt.sHtML

[R51] 排序去重取前几
来源：http://mobile.fktsv.cn/Article/details/gownxzirj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.sjlbkw.cn/Article/details/gerwupjwz.sHtML

[R52] 统计行数
来源：http://mobile.yfazqb.com/Article/details/gyzximkbt.sHtML

wc -l a.txt
来源：http://wap.fktsv.cn/Article/details/gvyxyheff.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fktsv.cn/Article/details/gmqbabwjt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.tarul.cn/Article/details/gwthtegce.sHtML

[R54] 比较两个文件
来源：http://www.blog.yfazqb.com/Article/details/gqyyjhhzy.sHtML

diff a.txt b.txt
来源：http://www.m.share.fktsv.cn/Article/details/ghzfydwns.sHtML

[R55] 压缩与解压
来源：http://3g.fktsv.cn/Article/details/gyhybxwtp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.vehdjk.com/Article/details/gxcyqquyh.sHtML

[R56] 远程拷贝
来源：http://read.share.bbcook.cn/Article/details/ggnwzoytc.sHtML

scp file user@host:/path/
来源：http://mobile.tarul.cn/Article/details/ggmgiyyue.sHtML

[R57] 远程执行命令
来源：http://baike.epnwcf.com/Article/details/gjwttvqsg.sHtML

ssh user@host 'uptime'
来源：http://baike.tarul.cn/Article/details/gskutlcrb.sHtML

[R58] 下载文件
来源：http://www.m.share.yfazqb.com/Article/details/gbunaxwam.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.bbcook.cn/Article/details/gstzykxtx.sHtML

[R59] 发 POST JSON
来源：http://read.share.epnwcf.com/Article/details/gmjuunofc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.sjlbkw.cn/Article/details/ghdjitvqo.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.epnwcf.com/Article/details/grpsjdxkc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fktsv.cn/Article/details/gwbaypusg.sHtML

[R61] 磁盘占用
来源：http://3g.tarul.cn/Article/details/gbqopthjz.sHtML

df -h;  du -sh *
来源：http://wap.epnwcf.com/Article/details/gnbebzlip.sHtML

[R62] 找最占空间的文件
来源：http://blog.tarul.cn/Article/details/gtzttuxhn.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.tarul.cn/Article/details/gohsvunji.sHtML

[R63] 内存与进程
来源：http://baike.epnwcf.com/Article/details/gmkrwcxjh.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.epnwcf.com/Article/details/gnvfyaiez.sHtML

[R64] 结束进程
来源：http://m.share.sjlbkw.cn/Article/details/gziihxcbb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fktsv.cn/Article/details/gbvsnlebm.sHtML

[R65] 查看端口占用
来源：http://m.share.epnwcf.com/Article/details/gkaiavrgn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.vehdjk.com/Article/details/gculsliio.sHtML

[R66] 定时任务
来源：http://www.share.bbcook.cn/Article/details/gedtxutlv.sHtML

crontab -e;  crontab -l
来源：http://3g.tarul.cn/Article/details/goshgcdrf.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.vehdjk.com/Article/details/garfchtwz.sHtML

openssl rand -hex 16
来源：http://3g.yfazqb.com/Article/details/gqrnbtosr.sHtML

[R68] 计算文件校验值
来源：http://www.share.fktsv.cn/Article/details/gyjhihftz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fktsv.cn/Article/details/goxwmebtt.sHtML

[R69] 生成随机密码
来源：http://mobile.sjlbkw.cn/Article/details/ghsozzhhd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.vehdjk.com/Article/details/gthyqeosk.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/geacuovrs.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.yfazqb.com/Article/details/gfrwzdhng.sHtML

[R71] 日期格式化
来源：http://wap.sjlbkw.cn/Article/details/giwqgyicl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.sjlbkw.cn/Article/details/gpjckmpkw.sHtML

[R72] 等待端口就绪
来源：http://www.share.sjlbkw.cn/Article/details/gmlgylogm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.sjlbkw.cn/Article/details/gzcpjlmfn.sHtML

[R73] 分割大日志
来源：http://wap.tarul.cn/Article/details/gdleomwfl.sHtML

split -l 1000 big.log part_
来源：http://m.share.fktsv.cn/Article/details/glnwqiild.sHtML

[R74] 批量重命名
来源：http://baike.epnwcf.com/Article/details/gzljfboht.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzirryjm.sHtML

[R75] 导出环境变量
来源：http://3g.fktsv.cn/Article/details/gisjuzmoq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.sjlbkw.cn/Article/details/gwamxjhda.sHtML

[R76] 使用临时文件
来源：http://www.share.epnwcf.com/Article/details/grbaalswn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gnjcgvrnp.sHtML

[R77] 读取用户输入
来源：http://www.share.sjlbkw.cn/Article/details/grdgykbgl.sHtML

read -rp "请输入: " ans
来源：http://blog.fktsv.cn/Article/details/gkvanfava.sHtML

[R78] 交互式菜单
来源：http://www.share.bbcook.cn/Article/details/gwomhwwuk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.bbcook.cn/Article/details/gfonojqkx.sHtML

[R79] 解析命令行选项
来源：http://3g.yfazqb.com/Article/details/gechzvxaj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.vehdjk.com/Article/details/galvsycaa.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.bbcook.cn/Article/details/gsxjitarn.sHtML

time ./run.sh
来源：http://3g.epnwcf.com/Article/details/gefrajnzz.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gezycxglu.sHtML

S. C / C++ 专题
来源：http://www.m.share.vehdjk.com/Article/details/gazyosqjp.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gmfxjlsea.sHtML

[S01] C：Hello World
来源：http://m.share.tarul.cn/Article/details/ghikiwhvr.sHtML

#include <stdio.h>
来源：http://m.share.bbcook.cn/Article/details/gqwhbfmwa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.vehdjk.com/Article/details/gjfnvotub.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.vehdjk.com/Article/details/gqxjybvkf.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.vehdjk.com/Article/details/grqrlqxul.sHtML

[S03] C：读入整数
来源：http://www.blog.tarul.cn/Article/details/gbzmtcuzo.sHtML

int x; scanf("%d", &x);
来源：http://read.share.epnwcf.com/Article/details/gpwvmebza.sHtML

[S04] C：字符串复制
来源：http://wap.bbcook.cn/Article/details/ggcxzeldh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.vehdjk.com/Article/details/gtybwoiai.sHtML

[S05] C：字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gxkeogohf.sHtML

strlen(s)
来源：http://read.share.bbcook.cn/Article/details/gublulbxl.sHtML

[S06] C：字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gmfcxaevp.sHtML

strcmp(a, b) == 0
来源：http://baike.yfazqb.com/Article/details/gzllqieit.sHtML

[S07] C：数组遍历求和
来源：http://3g.yfazqb.com/Article/details/gzpoyvqqy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.bbcook.cn/Article/details/gavryunja.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.yfazqb.com/Article/details/gwmowdalo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.yfazqb.com/Article/details/gwanhnudg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.sjlbkw.cn/Article/details/gubylyryd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.vehdjk.com/Article/details/gojzmmcxk.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.yfazqb.com/Article/details/glpofudif.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.epnwcf.com/Article/details/gslilxyrp.sHtML

[S11] C：逐行读文件
来源：http://baike.vehdjk.com/Article/details/gxemmpnsg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.epnwcf.com/Article/details/gyvfzmhfy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.sjlbkw.cn/Article/details/ggnqvlhzl.sHtML

fclose(f);
来源：http://3g.tarul.cn/Article/details/gfufwpfja.sHtML

[S12] C：写文件
来源：http://3g.tarul.cn/Article/details/gjgvvgfmu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/gopranypj.sHtML

[S13] C：宏定义
来源：http://read.share.sjlbkw.cn/Article/details/gumuhgzmm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.bbcook.cn/Article/details/gqsqasvzb.sHtML

[S14] C：枚举
来源：http://mobile.tarul.cn/Article/details/gvfwayhyu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.tarul.cn/Article/details/gzmgzsqrs.sHtML

[S15] C：类型转换
来源：http://mobile.vehdjk.com/Article/details/gwsgcourt.sHtML

(double) a / b
来源：http://www.share.fktsv.cn/Article/details/gvaadrvda.sHtML

[S16] C：位操作置位
来源：http://www.blog.yfazqb.com/Article/details/gmnhcuybn.sHtML

x |= (1 << 3);
来源：http://blog.bbcook.cn/Article/details/gusexgldy.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.yfazqb.com/Article/details/gpasopywb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.bbcook.cn/Article/details/gczftqqop.sHtML

[S18] C：命令行参数
来源：http://blog.epnwcf.com/Article/details/gyxoysqbw.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.bbcook.cn/Article/details/gxcvaobhf.sHtML

[S19] C：快速排序
来源：http://www.share.fktsv.cn/Article/details/gmcctvdpv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/getuwqfkr.sHtML

[S20] C：二分查找
来源：http://www.share.vehdjk.com/Article/details/gnsspwedp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/gzcimwdhw.sHtML

[S21] C：字符类别判断
来源：http://read.share.vehdjk.com/Article/details/gdfusuujx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.vehdjk.com/Article/details/ghltyrnuk.sHtML

[S22] C：字符串转数字
来源：http://baike.bbcook.cn/Article/details/gvjvvgvrs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.vehdjk.com/Article/details/ggdxyfeof.sHtML

[S23] C：随机数
来源：http://www.share.yfazqb.com/Article/details/glcuwlkdl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.vehdjk.com/Article/details/ggtidbuqa.sHtML

[S24] C：获取本地时间
来源：http://blog.epnwcf.com/Article/details/gizwtbuta.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.tarul.cn/Article/details/gytnyakkn.sHtML

[S25] C：内存拷贝
来源：http://mobile.vehdjk.com/Article/details/gencjzoto.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.epnwcf.com/Article/details/gfmwtxnnh.sHtML

[S26] C：内存清零
来源：http://www.share.fktsv.cn/Article/details/gsqkiasyq.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.yfazqb.com/Article/details/geyyrhlnr.sHtML

[S27] C：定义常量
来源：http://blog.yfazqb.com/Article/details/gqhmchcre.sHtML

const double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gxpkdykkg.sHtML

[S28] C：静态变量
来源：http://m.share.yfazqb.com/Article/details/ggmqdqphz.sHtML

static int counter = 0;
来源：http://read.share.yfazqb.com/Article/details/gokqcsedt.sHtML

[S29] C：变参函数
来源：http://www.blog.yfazqb.com/Article/details/gwvljzwka.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.sjlbkw.cn/Article/details/gsvxhpwos.sHtML

[S30] C：头文件保护
来源：http://m.share.fktsv.cn/Article/details/gujzffbqr.sHtML

#ifndef X_H
来源：http://read.share.tarul.cn/Article/details/gcbkpnjwe.sHtML

#define X_H
来源：http://read.share.yfazqb.com/Article/details/guihbouxp.sHtML

#endif
来源：http://www.share.bbcook.cn/Article/details/gpdnvbqxw.sHtML

[S31] C++：Hello World
来源：http://3g.fktsv.cn/Article/details/gitszhjhn.sHtML

#include <iostream>
来源：http://blog.tarul.cn/Article/details/gjerwvsvc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.tarul.cn/Article/details/grzxyhvrw.sHtML

[S32] C++：字符串
来源：http://3g.bbcook.cn/Article/details/gphlqugdj.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fktsv.cn/Article/details/ggqkptsdo.sHtML

[S33] C++：vector 增删
来源：http://read.share.vehdjk.com/Article/details/gvmsjusyd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fktsv.cn/Article/details/gkokxjgej.sHtML

[S34] C++：遍历 vector
来源：http://baike.sjlbkw.cn/Article/details/guckyebog.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fktsv.cn/Article/details/gxafofhnx.sHtML

[S35] C++：map
来源：http://baike.bbcook.cn/Article/details/gvdqzadfm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gtmrjmrjc.sHtML

[S36] C++：unordered_map
来源：http://read.share.yfazqb.com/Article/details/gczghztmo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.tarul.cn/Article/details/gdpqdmmoi.sHtML

[S37] C++：set
来源：http://3g.yfazqb.com/Article/details/gytundbts.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fktsv.cn/Article/details/gtjlhuemx.sHtML

[S38] C++：排序
来源：http://m.share.yfazqb.com/Article/details/gbdcczwpa.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.epnwcf.com/Article/details/grkeatjis.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.bbcook.cn/Article/details/gxgfegnti.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.bbcook.cn/Article/details/gmvxfurhu.sHtML

[S40] C++：查找元素
来源：http://read.share.fktsv.cn/Article/details/gjooqklse.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.bbcook.cn/Article/details/ggcjpesqh.sHtML

[S41] C++：类与构造函数
来源：http://read.share.vehdjk.com/Article/details/gvuftnhky.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.yfazqb.com/Article/details/giuvhvdvc.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.vehdjk.com/Article/details/gqeyfiucq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.tarul.cn/Article/details/gluwewpuf.sHtML

[S43] C++：智能指针
来源：http://3g.bbcook.cn/Article/details/ghmbadjju.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.sjlbkw.cn/Article/details/gvmvedebr.sHtML

[S44] C++：引用传参
来源：http://mobile.epnwcf.com/Article/details/gihvkgtpj.sHtML

void inc(int &x) { ++x; }
来源：http://blog.yfazqb.com/Article/details/grqmvhjby.sHtML

[S45] C++：lambda
来源：http://read.share.tarul.cn/Article/details/gbfdjdanr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.bbcook.cn/Article/details/gdyuysaaa.sHtML

[S46] C++：函数模板
来源：http://wap.epnwcf.com/Article/details/giyciywkg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.yfazqb.com/Article/details/gxwtrejyk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.epnwcf.com/Article/details/givvitbpu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkaauxsvi.sHtML

[S48] C++：逐行读文件
来源：http://blog.epnwcf.com/Article/details/geawokkrp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.epnwcf.com/Article/details/gqssubtaj.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.epnwcf.com/Article/details/gtsunkxvu.sHtML

[S49] C++：写文件
来源：http://wap.vehdjk.com/Article/details/gslluqdzi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fktsv.cn/Article/details/gqwefhrim.sHtML

[S50] C++：格式化数字
来源：http://www.blog.epnwcf.com/Article/details/gfyynhzxr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/ggdyxmqrd.sHtML

[S51] C++：显式类型转换
来源：http://3g.vehdjk.com/Article/details/gwsdjtawn.sHtML

static_cast<double>(a) / b
来源：http://3g.yfazqb.com/Article/details/gokuqwdxp.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fktsv.cn/Article/details/gfiztyboh.sHtML


<!-- 参考信息 -->