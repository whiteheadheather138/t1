代发 wailian999

[Q86] 读取 JSON 字段
来源：http://blog.fktsv.cn/Article/details/gxhykxtww.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.yfazqb.com/Article/details/grjklqkjx.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.bbcook.cn/Article/details/goxhskukr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.bbcook.cn/Article/details/ggwkltaqt.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.epnwcf.com/Article/details/guxnfdidk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.vehdjk.com/Article/details/glnezlzyk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.yfazqb.com/Article/details/gjdzoyifc.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.bbcook.cn/Article/details/gzpkuvrzo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.vehdjk.com/Article/details/govhnwnht.sHtML

[Q90] 生成序号列
来源：http://www.m.share.tarul.cn/Article/details/ghdlddmbq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fktsv.cn/Article/details/gbgcsxdme.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gjrzzfzfk.sHtML

R. Bash 专题
来源：http://mobile.vehdjk.com/Article/details/gcglxefxo.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gyafyucez.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.sjlbkw.cn/Article/details/gjugjcxca.sHtML

#!/usr/bin/env bash
来源：http://www.blog.vehdjk.com/Article/details/gevxjuezi.sHtML

set -euo pipefail
来源：http://m.share.yfazqb.com/Article/details/ganropwhi.sHtML

[R02] 变量赋值与使用
来源：http://read.share.yfazqb.com/Article/details/gdlfebzwt.sHtML

name="Tom"; echo "$name"
来源：http://blog.bbcook.cn/Article/details/gqivllqqj.sHtML

[R03] 只读变量
来源：http://baike.epnwcf.com/Article/details/grhblapqw.sHtML

readonly PI=3.14
来源：http://mobile.fktsv.cn/Article/details/gwfvoxtir.sHtML

[R04] 位置参数
来源：http://www.blog.vehdjk.com/Article/details/gaufanzlc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.epnwcf.com/Article/details/goevliiru.sHtML

[R05] 参数默认值
来源：http://www.blog.vehdjk.com/Article/details/ggqmbmmfp.sHtML

name="${1:-default}"
来源：http://www.share.fktsv.cn/Article/details/grcccsmtn.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fktsv.cn/Article/details/gbryjysgb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/gznzjynpi.sHtML

[R07] if 判断文件
来源：http://www.share.yfazqb.com/Article/details/gnywxqqhx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gzwuyvkcr.sHtML

[R08] 数值比较
来源：http://baike.vehdjk.com/Article/details/gncawetwy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.bbcook.cn/Article/details/gwfgcwhkj.sHtML

[R09] 字符串比较
来源：http://m.share.fktsv.cn/Article/details/giqnmnnui.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.yfazqb.com/Article/details/gwyppqbah.sHtML

[R10] 正则匹配
来源：http://read.share.sjlbkw.cn/Article/details/glbeoxbge.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fktsv.cn/Article/details/geefwpqpj.sHtML

[R11] case 多分支
来源：http://wap.bbcook.cn/Article/details/glkfkzbhf.sHtML

case "$1" in
来源：http://www.share.fktsv.cn/Article/details/gpoaqmavy.sHtML

start) echo "启动" ;;
来源：http://read.share.yfazqb.com/Article/details/gksrcacqk.sHtML

stop)  echo "停止" ;;
来源：http://wap.epnwcf.com/Article/details/gizdzfamn.sHtML

*)     echo "未知命令" ;;
来源：http://3g.tarul.cn/Article/details/gsvdczbas.sHtML

esac
来源：http://www.share.vehdjk.com/Article/details/grwyqfrkn.sHtML

[R12] for 遍历文件
来源：http://3g.vehdjk.com/Article/details/gsnuoeyue.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fktsv.cn/Article/details/gbckmydzw.sHtML

[R13] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/gzsqccoag.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/gmwbjajkw.sHtML

[R14] C 风格 for
来源：http://mobile.vehdjk.com/Article/details/gneviwfgk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/gfftlrxbm.sHtML

[R15] while 逐行读文件
来源：http://read.share.bbcook.cn/Article/details/glcnxjrkj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.sjlbkw.cn/Article/details/gjkmuuvqv.sHtML

[R16] until 等待条件
来源：http://m.share.sjlbkw.cn/Article/details/gkxgonlgw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.vehdjk.com/Article/details/ggjyaqayx.sHtML

[R17] 数组定义与取值
来源：http://m.share.fktsv.cn/Article/details/gvuzoqlnz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.epnwcf.com/Article/details/ghkhysclc.sHtML

[R18] 遍历数组
来源：http://3g.sjlbkw.cn/Article/details/glmznngee.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.yfazqb.com/Article/details/getzqowrr.sHtML

[R19] 数组长度
来源：http://m.share.vehdjk.com/Article/details/givpttejv.sHtML

echo "${#arr[@]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gypzpjscj.sHtML

[R20] 关联数组（字典）
来源：http://wap.bbcook.cn/Article/details/grfdgplvo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.vehdjk.com/Article/details/gowjczqgj.sHtML

[R21] 字符串长度
来源：http://m.share.epnwcf.com/Article/details/gyngdwben.sHtML

echo "${#s}"
来源：http://baike.bbcook.cn/Article/details/guidikgvm.sHtML

[R22] 截取子串
来源：http://m.share.yfazqb.com/Article/details/gpqedyjmn.sHtML

echo "${s:0:5}"
来源：http://mobile.sjlbkw.cn/Article/details/gkthefyjn.sHtML

[R23] 字符串替换
来源：http://3g.vehdjk.com/Article/details/gadnnsroy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.vehdjk.com/Article/details/glvvdeizr.sHtML

[R24] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/grentczup.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.bbcook.cn/Article/details/gzytdnrma.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.yfazqb.com/Article/details/gcyqcyimu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.sjlbkw.cn/Article/details/giwcppwsq.sHtML

[R26] 命令替换
来源：http://m.share.sjlbkw.cn/Article/details/gavpatzou.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.epnwcf.com/Article/details/gugvzbljg.sHtML

[R27] 算术展开
来源：http://www.m.share.vehdjk.com/Article/details/gutvrrbaa.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.tarul.cn/Article/details/gmdwuivdu.sHtML

[R28] 浮点运算
来源：http://read.share.bbcook.cn/Article/details/ggboopnoc.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.vehdjk.com/Article/details/ggfvaevaj.sHtML

[R29] 定义函数
来源：http://mobile.epnwcf.com/Article/details/gtigcrpwh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.epnwcf.com/Article/details/gstyxmlnd.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fktsv.cn/Article/details/gkqdwuvec.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.sjlbkw.cn/Article/details/gxzsawnuy.sHtML

[R31] 局部变量
来源：http://www.share.yfazqb.com/Article/details/ggwsalmrk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtxxngufp.sHtML

[R32] 参数个数校验
来源：http://mobile.epnwcf.com/Article/details/gpzdqskjf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/gzeqkndkb.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.sjlbkw.cn/Article/details/ghcvgsbud.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fktsv.cn/Article/details/gvhacmqtn.sHtML

[R34] 退出时清理
来源：http://www.m.share.epnwcf.com/Article/details/gyxeuwels.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gushnxipl.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.epnwcf.com/Article/details/gsrnxiczj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.epnwcf.com/Article/details/ggrfiitev.sHtML

[R36] 并发执行多个任务
来源：http://wap.fktsv.cn/Article/details/ggesifehr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.tarul.cn/Article/details/gsjvbefhs.sHtML

[R37] 把输出赋给变量
来源：http://3g.sjlbkw.cn/Article/details/gogppizjp.sHtML

files=$(ls -1)
来源：http://3g.sjlbkw.cn/Article/details/gharhpdlt.sHtML

[R38] 管道串联
来源：http://www.share.sjlbkw.cn/Article/details/gkxlkoign.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.vehdjk.com/Article/details/gdhkqlrps.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.epnwcf.com/Article/details/gofqwozex.sHtML

cmd > out.log 2>&1
来源：http://read.share.epnwcf.com/Article/details/gdzazrjpi.sHtML

[R40] 追加写日志
来源：http://3g.bbcook.cn/Article/details/gxdxebmrj.sHtML

echo "log" >> out.log
来源：http://www.m.share.bbcook.cn/Article/details/gtsvlvqnh.sHtML

[R41] 丢弃输出
来源：http://www.blog.epnwcf.com/Article/details/gcwakvfkq.sHtML

cmd >/dev/null 2>&1
来源：http://3g.yfazqb.com/Article/details/gcchqdizd.sHtML

[R42] 输入重定向
来源：http://baike.tarul.cn/Article/details/gcvyjzpse.sHtML

wc -l < a.txt
来源：http://m.share.yfazqb.com/Article/details/gaoeusrcl.sHtML

[R43] 按名字查找文件
来源：http://mobile.epnwcf.com/Article/details/gajjehzvi.sHtML

find . -name "*.log" -type f
来源：http://www.share.epnwcf.com/Article/details/gcmjohton.sHtML

[R44] 按修改时间查找
来源：http://mobile.tarul.cn/Article/details/gtmiqydcu.sHtML

find . -mtime -7 -type f
来源：http://www.blog.yfazqb.com/Article/details/ghcggbqvt.sHtML

[R45] 批量删除
来源：http://3g.yfazqb.com/Article/details/gxjrlyfeo.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.sjlbkw.cn/Article/details/gmxegsezd.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.epnwcf.com/Article/details/gmnlysvic.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.yfazqb.com/Article/details/gyigcwwrl.sHtML

[R47] sed 单行替换
来源：http://wap.yfazqb.com/Article/details/gavvnjles.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.epnwcf.com/Article/details/ghdubqgos.sHtML

[R48] awk 取指定列
来源：http://mobile.tarul.cn/Article/details/gxxbnlmsu.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.bbcook.cn/Article/details/gmpttbmsi.sHtML

[R49] awk 带条件
来源：http://www.share.yfazqb.com/Article/details/gzgcvmpul.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.sjlbkw.cn/Article/details/gzwqrmmlo.sHtML

[R50] awk 求和
来源：http://3g.vehdjk.com/Article/details/grnoespga.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.epnwcf.com/Article/details/ghujxxjma.sHtML

[R51] 排序去重取前几
来源：http://blog.tarul.cn/Article/details/gyguxhydq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.sjlbkw.cn/Article/details/grzdrdrdy.sHtML

[R52] 统计行数
来源：http://m.share.tarul.cn/Article/details/gbnftbvup.sHtML

wc -l a.txt
来源：http://www.blog.vehdjk.com/Article/details/gossaobdm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.epnwcf.com/Article/details/gubykjbug.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.sjlbkw.cn/Article/details/gkkfzegwm.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fktsv.cn/Article/details/gsqctykoq.sHtML

diff a.txt b.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gekrxenfi.sHtML

[R55] 压缩与解压
来源：http://www.blog.sjlbkw.cn/Article/details/gemlcklti.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fktsv.cn/Article/details/gskganmfl.sHtML

[R56] 远程拷贝
来源：http://3g.epnwcf.com/Article/details/gpvgqcxhx.sHtML

scp file user@host:/path/
来源：http://wap.epnwcf.com/Article/details/gnyporolf.sHtML

[R57] 远程执行命令
来源：http://www.blog.sjlbkw.cn/Article/details/gathcdipx.sHtML

ssh user@host 'uptime'
来源：http://baike.sjlbkw.cn/Article/details/gfzlnuzvw.sHtML

[R58] 下载文件
来源：http://read.share.bbcook.cn/Article/details/gmcuotkyd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.sjlbkw.cn/Article/details/gvooaocza.sHtML

[R59] 发 POST JSON
来源：http://read.share.yfazqb.com/Article/details/gohwolfln.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.bbcook.cn/Article/details/gneezfsbg.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/gfwvuiyzx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fktsv.cn/Article/details/gekkpgvfg.sHtML

[R61] 磁盘占用
来源：http://3g.yfazqb.com/Article/details/gepunjvez.sHtML

df -h;  du -sh *
来源：http://read.share.fktsv.cn/Article/details/gmvgvwgks.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.yfazqb.com/Article/details/ggusyotrp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.bbcook.cn/Article/details/glfzhalih.sHtML

[R63] 内存与进程
来源：http://www.blog.sjlbkw.cn/Article/details/gyokgumcs.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.sjlbkw.cn/Article/details/ghcgbaaoy.sHtML

[R64] 结束进程
来源：http://www.m.share.vehdjk.com/Article/details/gmdsntkfi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.bbcook.cn/Article/details/gluwnidjo.sHtML

[R65] 查看端口占用
来源：http://www.blog.epnwcf.com/Article/details/gazvwqueo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.yfazqb.com/Article/details/grngapepe.sHtML

[R66] 定时任务
来源：http://wap.yfazqb.com/Article/details/gwvfvkczt.sHtML

crontab -e;  crontab -l
来源：http://3g.yfazqb.com/Article/details/gkfhvuozv.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.bbcook.cn/Article/details/gisdnxgow.sHtML

openssl rand -hex 16
来源：http://read.share.tarul.cn/Article/details/gdihqltro.sHtML

[R68] 计算文件校验值
来源：http://www.share.sjlbkw.cn/Article/details/grpbrurfo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fktsv.cn/Article/details/gwcizwekj.sHtML

[R69] 生成随机密码
来源：http://blog.yfazqb.com/Article/details/gwjiaavjm.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.yfazqb.com/Article/details/gimvmkiow.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.vehdjk.com/Article/details/gwqchhtvg.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.vehdjk.com/Article/details/glsjfqywh.sHtML

[R71] 日期格式化
来源：http://www.blog.bbcook.cn/Article/details/giagzuqrr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.tarul.cn/Article/details/ghtrbqmsw.sHtML

[R72] 等待端口就绪
来源：http://www.share.yfazqb.com/Article/details/gzomjwpet.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.bbcook.cn/Article/details/gtburrodh.sHtML

[R73] 分割大日志
来源：http://www.blog.fktsv.cn/Article/details/gdiqgourf.sHtML

split -l 1000 big.log part_
来源：http://3g.sjlbkw.cn/Article/details/gyqyjczxd.sHtML

[R74] 批量重命名
来源：http://baike.sjlbkw.cn/Article/details/gultihhop.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.tarul.cn/Article/details/gideondyg.sHtML

[R75] 导出环境变量
来源：http://www.blog.yfazqb.com/Article/details/gqurmjwil.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.bbcook.cn/Article/details/gflumfptv.sHtML

[R76] 使用临时文件
来源：http://blog.tarul.cn/Article/details/ggmsnvszb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gtcrntehg.sHtML

[R77] 读取用户输入
来源：http://www.m.share.epnwcf.com/Article/details/gojxzlzcw.sHtML

read -rp "请输入: " ans
来源：http://3g.fktsv.cn/Article/details/gfdvgfdut.sHtML

[R78] 交互式菜单
来源：http://wap.tarul.cn/Article/details/gkrrugasc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.epnwcf.com/Article/details/gjjpiljxc.sHtML

[R79] 解析命令行选项
来源：http://wap.epnwcf.com/Article/details/gfcnyqyeh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.epnwcf.com/Article/details/grdmpabwa.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fktsv.cn/Article/details/gcuzbkbiu.sHtML

time ./run.sh
来源：http://3g.fktsv.cn/Article/details/gbgxudsoh.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guyhojilr.sHtML

S. C / C++ 专题
来源：http://m.share.yfazqb.com/Article/details/gtlusttmi.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gmgafplls.sHtML

[S01] C：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/geijvimox.sHtML

#include <stdio.h>
来源：http://read.share.bbcook.cn/Article/details/gzttbfskr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.tarul.cn/Article/details/gdfthtyim.sHtML

[S02] C：变量与格式化输出
来源：http://baike.bbcook.cn/Article/details/gcjrvbxhl.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.tarul.cn/Article/details/gxwmxaahn.sHtML

[S03] C：读入整数
来源：http://www.m.share.sjlbkw.cn/Article/details/glaimddjw.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.tarul.cn/Article/details/gyhbqhyhf.sHtML

[S04] C：字符串复制
来源：http://www.m.share.sjlbkw.cn/Article/details/gklhgagqk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gizwaqolh.sHtML

[S05] C：字符串长度
来源：http://mobile.vehdjk.com/Article/details/gwqgguzec.sHtML

strlen(s)
来源：http://blog.fktsv.cn/Article/details/gpolgssph.sHtML

[S06] C：字符串比较
来源：http://www.blog.fktsv.cn/Article/details/gcnojdsch.sHtML

strcmp(a, b) == 0
来源：http://m.share.vehdjk.com/Article/details/glkuvnpeh.sHtML

[S07] C：数组遍历求和
来源：http://3g.yfazqb.com/Article/details/gfmdkjfeu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.bbcook.cn/Article/details/gmwwktlwd.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.yfazqb.com/Article/details/gjjxqmsop.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fktsv.cn/Article/details/gnycjgakl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzjzurzi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.tarul.cn/Article/details/gmnjbhmkh.sHtML

[S10] C：指针与解引用
来源：http://read.share.fktsv.cn/Article/details/gauaxbsxa.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.vehdjk.com/Article/details/gvvbuyrso.sHtML

[S11] C：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gyyibgwjg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.vehdjk.com/Article/details/gyzwprzan.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.bbcook.cn/Article/details/gdxjjylvr.sHtML

fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/glmswxzwx.sHtML

[S12] C：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gxusruzsz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.bbcook.cn/Article/details/gmiolanef.sHtML

[S13] C：宏定义
来源：http://baike.sjlbkw.cn/Article/details/gnzexsbbk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.tarul.cn/Article/details/gjulhmkdl.sHtML

[S14] C：枚举
来源：http://www.m.share.yfazqb.com/Article/details/gfojhtqoc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.vehdjk.com/Article/details/gwmmeyfyp.sHtML

[S15] C：类型转换
来源：http://3g.fktsv.cn/Article/details/guspboxqe.sHtML

(double) a / b
来源：http://3g.sjlbkw.cn/Article/details/gxkbhtvmz.sHtML

[S16] C：位操作置位
来源：http://www.blog.epnwcf.com/Article/details/gfmimkfuh.sHtML

x |= (1 << 3);
来源：http://m.share.vehdjk.com/Article/details/ghxxzxhdu.sHtML

[S17] C：安全拼接字符串
来源：http://baike.tarul.cn/Article/details/gdnlcqbkw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.epnwcf.com/Article/details/gjttdvphl.sHtML

[S18] C：命令行参数
来源：http://mobile.fktsv.cn/Article/details/gghwsvneq.sHtML

int main(int argc, char **argv)
来源：http://mobile.bbcook.cn/Article/details/gxecpukaa.sHtML

[S19] C：快速排序
来源：http://wap.tarul.cn/Article/details/grzmetuwn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gtgwpelfm.sHtML

[S20] C：二分查找
来源：http://wap.tarul.cn/Article/details/gpouekvoo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/gpziwvjts.sHtML

[S21] C：字符类别判断
来源：http://3g.yfazqb.com/Article/details/glgfwaoqh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fktsv.cn/Article/details/gxmeeeydn.sHtML

[S22] C：字符串转数字
来源：http://read.share.bbcook.cn/Article/details/gtgsgtyeo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.yfazqb.com/Article/details/gfzdvxxzg.sHtML

[S23] C：随机数
来源：http://3g.vehdjk.com/Article/details/goizflisi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.bbcook.cn/Article/details/gexroiscs.sHtML

[S24] C：获取本地时间
来源：http://blog.epnwcf.com/Article/details/gzlkpihoo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.vehdjk.com/Article/details/ggdcafnpm.sHtML

[S25] C：内存拷贝
来源：http://wap.epnwcf.com/Article/details/gitjrdzwf.sHtML

memcpy(dst, src, n);
来源：http://www.blog.yfazqb.com/Article/details/gperjidkc.sHtML

[S26] C：内存清零
来源：http://m.share.vehdjk.com/Article/details/gnivimigw.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.sjlbkw.cn/Article/details/gshupndwt.sHtML

[S27] C：定义常量
来源：http://3g.epnwcf.com/Article/details/gseilaqao.sHtML

const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gdmkadceq.sHtML

[S28] C：静态变量
来源：http://read.share.fktsv.cn/Article/details/gtumaktht.sHtML

static int counter = 0;
来源：http://baike.fktsv.cn/Article/details/gqznvtmjq.sHtML

[S29] C：变参函数
来源：http://blog.epnwcf.com/Article/details/glkmsdoxv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.vehdjk.com/Article/details/gowinqhdq.sHtML

[S30] C：头文件保护
来源：http://www.m.share.bbcook.cn/Article/details/grzfeefia.sHtML

#ifndef X_H
来源：http://baike.tarul.cn/Article/details/gaoedmstv.sHtML

#define X_H
来源：http://www.m.share.epnwcf.com/Article/details/gqdzkgeea.sHtML

#endif
来源：http://mobile.vehdjk.com/Article/details/gvgrprrlu.sHtML

[S31] C++：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/ggncnqalf.sHtML

#include <iostream>
来源：http://baike.epnwcf.com/Article/details/gzwajqpnb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.yfazqb.com/Article/details/ghzbvcnnz.sHtML

[S32] C++：字符串
来源：http://www.blog.vehdjk.com/Article/details/gblnnwxqi.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.sjlbkw.cn/Article/details/geescpmfh.sHtML

[S33] C++：vector 增删
来源：http://blog.fktsv.cn/Article/details/gfwmgabba.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.epnwcf.com/Article/details/gvmgzjkfy.sHtML

[S34] C++：遍历 vector
来源：http://baike.yfazqb.com/Article/details/ggqyiqpbb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.epnwcf.com/Article/details/gksmuguge.sHtML

[S35] C++：map
来源：http://baike.sjlbkw.cn/Article/details/gxywsrmzn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/gmincdmff.sHtML

[S36] C++：unordered_map
来源：http://www.share.sjlbkw.cn/Article/details/gumijazoy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.yfazqb.com/Article/details/guncjtlku.sHtML

[S37] C++：set
来源：http://read.share.bbcook.cn/Article/details/gxokvpoxw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.tarul.cn/Article/details/gcncxceog.sHtML

[S38] C++：排序
来源：http://www.share.epnwcf.com/Article/details/ggurkfrpu.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.bbcook.cn/Article/details/gzvoganep.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.tarul.cn/Article/details/ggmqafbdu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fktsv.cn/Article/details/gbvilqziu.sHtML

[S40] C++：查找元素
来源：http://baike.bbcook.cn/Article/details/glsphsvlq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.vehdjk.com/Article/details/gqtvpsseh.sHtML

[S41] C++：类与构造函数
来源：http://baike.epnwcf.com/Article/details/gtxipawrv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.sjlbkw.cn/Article/details/gqcmurzyl.sHtML

[S42] C++：继承与虚函数
来源：http://3g.sjlbkw.cn/Article/details/gnwvtrmpu.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.vehdjk.com/Article/details/gxlvnlzzk.sHtML

[S43] C++：智能指针
来源：http://blog.fktsv.cn/Article/details/gcvmuhung.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.tarul.cn/Article/details/geowomkuu.sHtML

[S44] C++：引用传参
来源：http://mobile.epnwcf.com/Article/details/gjorkbldk.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fktsv.cn/Article/details/gebrwusbu.sHtML

[S45] C++：lambda
来源：http://baike.fktsv.cn/Article/details/ggftdzdhx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.vehdjk.com/Article/details/gboyeqekc.sHtML

[S46] C++：函数模板
来源：http://3g.sjlbkw.cn/Article/details/gvkdewuxb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.vehdjk.com/Article/details/guifzvhhh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.bbcook.cn/Article/details/giyiuwmgt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.tarul.cn/Article/details/grikbomzi.sHtML

[S48] C++：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gxqspfobe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.bbcook.cn/Article/details/griyinmsk.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.tarul.cn/Article/details/ggxugoexr.sHtML

[S49] C++：写文件
来源：http://www.share.bbcook.cn/Article/details/gzeegqptc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.tarul.cn/Article/details/gmwnrixih.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.bbcook.cn/Article/details/gjdpnvarw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fktsv.cn/Article/details/glyycfqmw.sHtML

[S51] C++：显式类型转换
来源：http://blog.fktsv.cn/Article/details/gndcepflu.sHtML

static_cast<double>(a) / b
来源：http://3g.yfazqb.com/Article/details/gmydxchmy.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.yfazqb.com/Article/details/gxyugwrpe.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.bbcook.cn/Article/details/gatvgwqco.sHtML

[S53] C++：移动语义
来源：http://www.share.tarul.cn/Article/details/gjrscsbws.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.epnwcf.com/Article/details/glchutscy.sHtML

[S54] C++：异常处理
来源：http://m.share.tarul.cn/Article/details/gvkgwinkn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.tarul.cn/Article/details/givejuqmv.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.epnwcf.com/Article/details/gwlksxqym.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fktsv.cn/Article/details/ghxpkgvoc.sHtML

[S56] C++：optional
来源：http://www.blog.fktsv.cn/Article/details/gbdoosezv.sHtML


<!-- 参考信息 -->