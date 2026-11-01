代发 wailian999

[Q82] 字符长度与字节长度
来源：http://blog.fktsv.cn/Article/details/gsfasyyte.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gvwemisua.sHtML

[Q83] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/glmojvlke.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gchlmzesn.sHtML

[Q84] 去除首尾空格
来源：http://baike.sjlbkw.cn/Article/details/ggxdnbfvl.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/giasozwcn.sHtML

[Q85] 数值取整
来源：http://m.share.epnwcf.com/Article/details/gjfxsmbsr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fktsv.cn/Article/details/grjrlkxxi.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.yfazqb.com/Article/details/gdhdrtxke.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.vehdjk.com/Article/details/gssyayife.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.bbcook.cn/Article/details/glqriyjev.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.epnwcf.com/Article/details/gjsiwubxy.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fktsv.cn/Article/details/gigcuxmmb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.vehdjk.com/Article/details/gwilxxwlx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.epnwcf.com/Article/details/gsetlophj.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.tarul.cn/Article/details/gntfbafor.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fktsv.cn/Article/details/gqxgurjeh.sHtML

[Q90] 生成序号列
来源：http://www.m.share.vehdjk.com/Article/details/gstedakuf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.epnwcf.com/Article/details/gmyfvnahy.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gnohhpjlt.sHtML

R. Bash 专题
来源：http://read.share.fktsv.cn/Article/details/gmkxjyghu.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gitkmychl.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.vehdjk.com/Article/details/gobqohswg.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.sjlbkw.cn/Article/details/gigyydsod.sHtML

set -euo pipefail
来源：http://baike.yfazqb.com/Article/details/gdrcbelab.sHtML

[R02] 变量赋值与使用
来源：http://m.share.tarul.cn/Article/details/gmnbujscg.sHtML

name="Tom"; echo "$name"
来源：http://mobile.sjlbkw.cn/Article/details/gguhqrbxx.sHtML

[R03] 只读变量
来源：http://blog.sjlbkw.cn/Article/details/gdrealujx.sHtML

readonly PI=3.14
来源：http://3g.fktsv.cn/Article/details/gecmbitrh.sHtML

[R04] 位置参数
来源：http://wap.yfazqb.com/Article/details/glvzknswk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.vehdjk.com/Article/details/gzhpszhip.sHtML

[R05] 参数默认值
来源：http://read.share.tarul.cn/Article/details/gqgmwjrzw.sHtML

name="${1:-default}"
来源：http://mobile.bbcook.cn/Article/details/grjotycjo.sHtML

[R06] 判断命令是否存在
来源：http://blog.bbcook.cn/Article/details/ggnregnxw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/gxdmeczll.sHtML

[R07] if 判断文件
来源：http://www.blog.yfazqb.com/Article/details/gpnyqepwc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fktsv.cn/Article/details/gnbonpwmk.sHtML

[R08] 数值比较
来源：http://m.share.tarul.cn/Article/details/gsywtppia.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.bbcook.cn/Article/details/gbelpijdk.sHtML

[R09] 字符串比较
来源：http://m.share.bbcook.cn/Article/details/gdvziqfrl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.vehdjk.com/Article/details/gslxukxqz.sHtML

[R10] 正则匹配
来源：http://www.blog.yfazqb.com/Article/details/glqtaacnb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fktsv.cn/Article/details/gvmguqlkx.sHtML

[R11] case 多分支
来源：http://mobile.epnwcf.com/Article/details/goqvepzud.sHtML

case "$1" in
来源：http://mobile.vehdjk.com/Article/details/gkhqhbovk.sHtML

start) echo "启动" ;;
来源：http://blog.epnwcf.com/Article/details/guwopcdqa.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.tarul.cn/Article/details/gmsolurbk.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fktsv.cn/Article/details/grebtpfxo.sHtML

esac
来源：http://blog.bbcook.cn/Article/details/grvgppfpn.sHtML

[R12] for 遍历文件
来源：http://baike.fktsv.cn/Article/details/getinsthb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.sjlbkw.cn/Article/details/gttnmoyay.sHtML

[R13] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/gwvxbevth.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.yfazqb.com/Article/details/gacsrqiwj.sHtML

[R14] C 风格 for
来源：http://mobile.epnwcf.com/Article/details/gtvnneqgi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gbryxates.sHtML

[R15] while 逐行读文件
来源：http://blog.yfazqb.com/Article/details/gnygzftgb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.sjlbkw.cn/Article/details/gnimqluod.sHtML

[R16] until 等待条件
来源：http://www.m.share.yfazqb.com/Article/details/gkzsrbnoz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/garumitsn.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fktsv.cn/Article/details/grwnoycgg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.sjlbkw.cn/Article/details/gdcpypdxb.sHtML

[R18] 遍历数组
来源：http://mobile.tarul.cn/Article/details/gzfpslzeh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fktsv.cn/Article/details/gjefleqir.sHtML

[R19] 数组长度
来源：http://3g.tarul.cn/Article/details/gzkacvfoj.sHtML

echo "${#arr[@]}"
来源：http://wap.yfazqb.com/Article/details/gtwgyfokm.sHtML

[R20] 关联数组（字典）
来源：http://read.share.sjlbkw.cn/Article/details/gmkbyxqgl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fktsv.cn/Article/details/ghctabaae.sHtML

[R21] 字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/grnlervfz.sHtML

echo "${#s}"
来源：http://baike.yfazqb.com/Article/details/gjmyjetnp.sHtML

[R22] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/gqpvsaxip.sHtML

echo "${s:0:5}"
来源：http://www.m.share.bbcook.cn/Article/details/gywlnpejr.sHtML

[R23] 字符串替换
来源：http://www.blog.sjlbkw.cn/Article/details/gnceknynh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.bbcook.cn/Article/details/gtsoamlhw.sHtML

[R24] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gkonezwny.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.vehdjk.com/Article/details/gytesnwdq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.vehdjk.com/Article/details/gkkmgvoqr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.bbcook.cn/Article/details/ggphgnqnv.sHtML

[R26] 命令替换
来源：http://wap.epnwcf.com/Article/details/gjxewtvvy.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.bbcook.cn/Article/details/gkwdvtbya.sHtML

[R27] 算术展开
来源：http://www.m.share.yfazqb.com/Article/details/guhrrhtlq.sHtML

echo $((1 + 2 * 3))
来源：http://wap.yfazqb.com/Article/details/gtbnkduaw.sHtML

[R28] 浮点运算
来源：http://baike.tarul.cn/Article/details/gcdbxkomz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.epnwcf.com/Article/details/gbufkqrqw.sHtML

[R29] 定义函数
来源：http://3g.bbcook.cn/Article/details/gvavrnpvy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.yfazqb.com/Article/details/gtcpqvojt.sHtML

[R30] 函数返回状态码
来源：http://baike.epnwcf.com/Article/details/gyfvqxwww.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fktsv.cn/Article/details/gbypqxblq.sHtML

[R31] 局部变量
来源：http://m.share.yfazqb.com/Article/details/gmngzrcrl.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.bbcook.cn/Article/details/gyeiixmxl.sHtML

[R32] 参数个数校验
来源：http://m.share.fktsv.cn/Article/details/gxotbemwd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/glfktrydg.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.yfazqb.com/Article/details/gqipfqqor.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fktsv.cn/Article/details/gwrypnprd.sHtML

[R34] 退出时清理
来源：http://read.share.tarul.cn/Article/details/gdmbpbnad.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fktsv.cn/Article/details/gzrcjzkpt.sHtML

[R35] 后台执行并等待
来源：http://mobile.epnwcf.com/Article/details/gesmvdvxd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.tarul.cn/Article/details/gfvonnczq.sHtML

[R36] 并发执行多个任务
来源：http://blog.fktsv.cn/Article/details/gvjjtetdx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fktsv.cn/Article/details/gnuujyjfp.sHtML

[R37] 把输出赋给变量
来源：http://wap.yfazqb.com/Article/details/gduyaetjw.sHtML

files=$(ls -1)
来源：http://wap.fktsv.cn/Article/details/gefvgdyiz.sHtML

[R38] 管道串联
来源：http://www.blog.bbcook.cn/Article/details/gwdfnnihb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.vehdjk.com/Article/details/gfynyxlqm.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fktsv.cn/Article/details/gdocrgmdg.sHtML

cmd > out.log 2>&1
来源：http://3g.bbcook.cn/Article/details/gwagfkcqb.sHtML

[R40] 追加写日志
来源：http://www.share.epnwcf.com/Article/details/gxsswjhmy.sHtML

echo "log" >> out.log
来源：http://m.share.yfazqb.com/Article/details/gnndqtwnz.sHtML

[R41] 丢弃输出
来源：http://read.share.yfazqb.com/Article/details/gbsehlruv.sHtML

cmd >/dev/null 2>&1
来源：http://baike.vehdjk.com/Article/details/gcpjcbgqz.sHtML

[R42] 输入重定向
来源：http://wap.bbcook.cn/Article/details/gbmknpwsl.sHtML

wc -l < a.txt
来源：http://wap.yfazqb.com/Article/details/gshadtkyd.sHtML

[R43] 按名字查找文件
来源：http://read.share.sjlbkw.cn/Article/details/guenziqht.sHtML

find . -name "*.log" -type f
来源：http://m.share.vehdjk.com/Article/details/grjauddje.sHtML

[R44] 按修改时间查找
来源：http://mobile.epnwcf.com/Article/details/gvveckntb.sHtML

find . -mtime -7 -type f
来源：http://mobile.tarul.cn/Article/details/gdngayvzl.sHtML

[R45] 批量删除
来源：http://baike.vehdjk.com/Article/details/gbqqdjzfa.sHtML

find . -name "*.tmp" -delete
来源：http://blog.epnwcf.com/Article/details/gfpsosiuj.sHtML

[R46] 递归替换文件内容
来源：http://wap.sjlbkw.cn/Article/details/gqzmoqknk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.sjlbkw.cn/Article/details/gijwoncsj.sHtML

[R47] sed 单行替换
来源：http://mobile.yfazqb.com/Article/details/gmcnqiucc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.bbcook.cn/Article/details/gawsbmsac.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fktsv.cn/Article/details/gukbdrgmi.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/ggugwyyep.sHtML

[R49] awk 带条件
来源：http://www.m.share.epnwcf.com/Article/details/gzohlsafp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.epnwcf.com/Article/details/ggxwsdbpg.sHtML

[R50] awk 求和
来源：http://baike.sjlbkw.cn/Article/details/glqwzpjwf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.bbcook.cn/Article/details/gxhviynjy.sHtML

[R51] 排序去重取前几
来源：http://www.share.tarul.cn/Article/details/gowqcvixy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.sjlbkw.cn/Article/details/gjbofmlwx.sHtML

[R52] 统计行数
来源：http://read.share.sjlbkw.cn/Article/details/gveaevywo.sHtML

wc -l a.txt
来源：http://baike.tarul.cn/Article/details/gxtbnwunv.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.bbcook.cn/Article/details/gtahibrbe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.bbcook.cn/Article/details/gjgcsfwcj.sHtML

[R54] 比较两个文件
来源：http://mobile.fktsv.cn/Article/details/gntdkwysl.sHtML

diff a.txt b.txt
来源：http://www.m.share.vehdjk.com/Article/details/gcdjdvhvx.sHtML

[R55] 压缩与解压
来源：http://3g.epnwcf.com/Article/details/gjpiobcrm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/gpevboliv.sHtML

[R56] 远程拷贝
来源：http://m.share.yfazqb.com/Article/details/glelygina.sHtML

scp file user@host:/path/
来源：http://read.share.sjlbkw.cn/Article/details/gjtjxzphx.sHtML

[R57] 远程执行命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkfeueho.sHtML

ssh user@host 'uptime'
来源：http://read.share.sjlbkw.cn/Article/details/gogqoocnu.sHtML

[R58] 下载文件
来源：http://m.share.bbcook.cn/Article/details/gbpzbtmda.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.vehdjk.com/Article/details/gnsqiasum.sHtML

[R59] 发 POST JSON
来源：http://blog.bbcook.cn/Article/details/gnskyolub.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.tarul.cn/Article/details/gxpqzqgek.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.epnwcf.com/Article/details/gbizpgxyt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.vehdjk.com/Article/details/grkxucozt.sHtML

[R61] 磁盘占用
来源：http://mobile.yfazqb.com/Article/details/grqifxcqp.sHtML

df -h;  du -sh *
来源：http://baike.yfazqb.com/Article/details/gzmmnxtrm.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fktsv.cn/Article/details/grlvxoqgg.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.bbcook.cn/Article/details/glghnldwy.sHtML

[R63] 内存与进程
来源：http://www.m.share.bbcook.cn/Article/details/gwlrkevex.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fktsv.cn/Article/details/gojpaqivh.sHtML

[R64] 结束进程
来源：http://m.share.fktsv.cn/Article/details/gljkkzfqy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.sjlbkw.cn/Article/details/gmewjxdac.sHtML

[R65] 查看端口占用
来源：http://3g.bbcook.cn/Article/details/gfajjpebh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.epnwcf.com/Article/details/gvmxqbdyh.sHtML

[R66] 定时任务
来源：http://www.share.sjlbkw.cn/Article/details/gbmmqmvit.sHtML

crontab -e;  crontab -l
来源：http://www.blog.epnwcf.com/Article/details/gidcdvjez.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.tarul.cn/Article/details/gmyciaqip.sHtML

openssl rand -hex 16
来源：http://wap.sjlbkw.cn/Article/details/gpufrfjgr.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.tarul.cn/Article/details/gjrnwnpov.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fktsv.cn/Article/details/gpzsecqpe.sHtML

[R69] 生成随机密码
来源：http://read.share.bbcook.cn/Article/details/gadwomcmu.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.epnwcf.com/Article/details/gymrqvnza.sHtML

[R70] 时间戳与互转
来源：http://read.share.sjlbkw.cn/Article/details/gxdfshojg.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.vehdjk.com/Article/details/gtlfupjcy.sHtML

[R71] 日期格式化
来源：http://m.share.sjlbkw.cn/Article/details/gxapqppno.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.vehdjk.com/Article/details/gmuhmtsff.sHtML

[R72] 等待端口就绪
来源：http://read.share.sjlbkw.cn/Article/details/ggjxekbgz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.sjlbkw.cn/Article/details/gkyjzwwgu.sHtML

[R73] 分割大日志
来源：http://baike.yfazqb.com/Article/details/gyrgjlohv.sHtML

split -l 1000 big.log part_
来源：http://www.share.yfazqb.com/Article/details/gyddqtucx.sHtML

[R74] 批量重命名
来源：http://mobile.yfazqb.com/Article/details/gxlozvrtd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.sjlbkw.cn/Article/details/gkzpqhyej.sHtML

[R75] 导出环境变量
来源：http://baike.bbcook.cn/Article/details/gqacrshbg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.sjlbkw.cn/Article/details/gttyttqzx.sHtML

[R76] 使用临时文件
来源：http://wap.sjlbkw.cn/Article/details/ggrglatds.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.epnwcf.com/Article/details/gohazbtvt.sHtML

[R77] 读取用户输入
来源：http://www.m.share.sjlbkw.cn/Article/details/gonqsjtzf.sHtML

read -rp "请输入: " ans
来源：http://m.share.vehdjk.com/Article/details/gxwpyrmmp.sHtML

[R78] 交互式菜单
来源：http://baike.bbcook.cn/Article/details/ghbnlyvtz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.sjlbkw.cn/Article/details/glxvaqzbc.sHtML

[R79] 解析命令行选项
来源：http://baike.bbcook.cn/Article/details/gkzxuhalf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.tarul.cn/Article/details/gxijctcgx.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fktsv.cn/Article/details/gbaoancvk.sHtML

time ./run.sh
来源：http://www.m.share.epnwcf.com/Article/details/gopqnztye.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gxjqcmoyd.sHtML

S. C / C++ 专题
来源：http://blog.sjlbkw.cn/Article/details/gakoygkwt.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghtfjhphg.sHtML

[S01] C：Hello World
来源：http://www.share.epnwcf.com/Article/details/goazygsvl.sHtML

#include <stdio.h>
来源：http://baike.fktsv.cn/Article/details/gsbwvcgnb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fktsv.cn/Article/details/gyqtumcnx.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.yfazqb.com/Article/details/gxmkmusrh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.epnwcf.com/Article/details/goebupqor.sHtML

[S03] C：读入整数
来源：http://www.share.bbcook.cn/Article/details/gfnuahddf.sHtML

int x; scanf("%d", &x);
来源：http://mobile.tarul.cn/Article/details/gujotntxd.sHtML

[S04] C：字符串复制
来源：http://mobile.yfazqb.com/Article/details/gbjabwjrd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.epnwcf.com/Article/details/gbfztpviv.sHtML

[S05] C：字符串长度
来源：http://baike.bbcook.cn/Article/details/gnwkawevc.sHtML

strlen(s)
来源：http://www.blog.bbcook.cn/Article/details/gcndsdzmx.sHtML

[S06] C：字符串比较
来源：http://wap.epnwcf.com/Article/details/garcrysqv.sHtML

strcmp(a, b) == 0
来源：http://read.share.yfazqb.com/Article/details/gerfbpujo.sHtML

[S07] C：数组遍历求和
来源：http://wap.vehdjk.com/Article/details/gcstzldkr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.epnwcf.com/Article/details/gqoojyhxq.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.tarul.cn/Article/details/guhkiwuiw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.yfazqb.com/Article/details/ggiyhdwoc.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.tarul.cn/Article/details/gqkilnrtx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.vehdjk.com/Article/details/gxvlidjnu.sHtML

[S10] C：指针与解引用
来源：http://www.share.sjlbkw.cn/Article/details/gttiujsaz.sHtML

int *p = &a;  *p = 5;
来源：http://blog.tarul.cn/Article/details/ggifdlwjc.sHtML

[S11] C：逐行读文件
来源：http://3g.yfazqb.com/Article/details/guvfckcwx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.epnwcf.com/Article/details/goezovlsr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.yfazqb.com/Article/details/gduochibd.sHtML

fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/gucfpdnie.sHtML

[S12] C：写文件
来源：http://www.share.tarul.cn/Article/details/gfmxfibly.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/gnbwtfygp.sHtML

[S13] C：宏定义
来源：http://m.share.yfazqb.com/Article/details/gwromzepk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.yfazqb.com/Article/details/gbrkqkutm.sHtML

[S14] C：枚举
来源：http://baike.sjlbkw.cn/Article/details/gtaditxgr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.yfazqb.com/Article/details/givvcfjnl.sHtML

[S15] C：类型转换
来源：http://3g.vehdjk.com/Article/details/gqvmwvjba.sHtML

(double) a / b
来源：http://3g.tarul.cn/Article/details/gagjyfuxn.sHtML

[S16] C：位操作置位
来源：http://read.share.tarul.cn/Article/details/gswpzastk.sHtML

x |= (1 << 3);
来源：http://www.share.vehdjk.com/Article/details/glyjqgxfp.sHtML

[S17] C：安全拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/ghnozrggc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.tarul.cn/Article/details/gvduyjngi.sHtML

[S18] C：命令行参数
来源：http://mobile.fktsv.cn/Article/details/gwqdsuqrs.sHtML

int main(int argc, char **argv)
来源：http://www.share.yfazqb.com/Article/details/gcjpczpig.sHtML

[S19] C：快速排序
来源：http://m.share.fktsv.cn/Article/details/gcomezmrp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/ggmkbmewb.sHtML

[S20] C：二分查找
来源：http://www.blog.epnwcf.com/Article/details/glbairzsl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.yfazqb.com/Article/details/gwnigwpdf.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.vehdjk.com/Article/details/gnsgbotem.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.yfazqb.com/Article/details/gansjwqrf.sHtML

[S22] C：字符串转数字
来源：http://3g.vehdjk.com/Article/details/gttqbsvgn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.epnwcf.com/Article/details/gpvvrpphn.sHtML

[S23] C：随机数
来源：http://www.m.share.bbcook.cn/Article/details/gvseoxqpf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.epnwcf.com/Article/details/golpnnbqx.sHtML

[S24] C：获取本地时间
来源：http://wap.epnwcf.com/Article/details/gxohtlruf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.vehdjk.com/Article/details/gvigwcmdj.sHtML

[S25] C：内存拷贝
来源：http://m.share.fktsv.cn/Article/details/gtotdswbb.sHtML

memcpy(dst, src, n);
来源：http://read.share.bbcook.cn/Article/details/guznqdnfs.sHtML

[S26] C：内存清零
来源：http://blog.fktsv.cn/Article/details/gdcigvtfj.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.epnwcf.com/Article/details/gfriokozo.sHtML

[S27] C：定义常量
来源：http://www.share.tarul.cn/Article/details/gshoesqcr.sHtML

const double PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/ghtpwecvz.sHtML

[S28] C：静态变量
来源：http://m.share.bbcook.cn/Article/details/gtfbdmjpi.sHtML

static int counter = 0;
来源：http://m.share.bbcook.cn/Article/details/ghcwgbfod.sHtML

[S29] C：变参函数
来源：http://3g.bbcook.cn/Article/details/gwmkdxwvv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.vehdjk.com/Article/details/gxsklqdjl.sHtML

[S30] C：头文件保护
来源：http://www.blog.vehdjk.com/Article/details/gwkkgyksr.sHtML

#ifndef X_H
来源：http://m.share.vehdjk.com/Article/details/gnfjpplaj.sHtML

#define X_H
来源：http://www.share.fktsv.cn/Article/details/gcudbycdk.sHtML

#endif
来源：http://www.m.share.bbcook.cn/Article/details/gbjcgnmxn.sHtML

[S31] C++：Hello World
来源：http://wap.epnwcf.com/Article/details/gakemrons.sHtML

#include <iostream>
来源：http://www.m.share.epnwcf.com/Article/details/gyyczslin.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.yfazqb.com/Article/details/gwextjoka.sHtML

[S32] C++：字符串
来源：http://baike.bbcook.cn/Article/details/ghghxtwus.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.bbcook.cn/Article/details/glaneliyf.sHtML

[S33] C++：vector 增删
来源：http://3g.vehdjk.com/Article/details/gsdzppagq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.tarul.cn/Article/details/gecvmvvhv.sHtML

[S34] C++：遍历 vector
来源：http://www.share.sjlbkw.cn/Article/details/gxbeqvibz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrtuakda.sHtML

[S35] C++：map
来源：http://www.m.share.epnwcf.com/Article/details/guhmdayta.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.tarul.cn/Article/details/gbklqtjbq.sHtML

[S36] C++：unordered_map
来源：http://baike.yfazqb.com/Article/details/gsnhujwmj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gzwzqmrcj.sHtML

[S37] C++：set
来源：http://mobile.bbcook.cn/Article/details/gejzlmmcg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.yfazqb.com/Article/details/gniumsska.sHtML

[S38] C++：排序
来源：http://3g.yfazqb.com/Article/details/gpvvmptqr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.tarul.cn/Article/details/gftvrkmyn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.bbcook.cn/Article/details/gwpzgimmc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.sjlbkw.cn/Article/details/gaaayhlox.sHtML

[S40] C++：查找元素
来源：http://read.share.epnwcf.com/Article/details/gbhjyfgrh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.yfazqb.com/Article/details/gtolsnzib.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fktsv.cn/Article/details/ggmxpbifn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.epnwcf.com/Article/details/gmkdldbol.sHtML

[S42] C++：继承与虚函数
来源：http://blog.yfazqb.com/Article/details/giboqbblb.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.epnwcf.com/Article/details/gtqlaozwy.sHtML

[S43] C++：智能指针
来源：http://www.share.tarul.cn/Article/details/guhpubfgv.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.epnwcf.com/Article/details/gntoeyvff.sHtML

[S44] C++：引用传参
来源：http://wap.tarul.cn/Article/details/gumihkgwy.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fktsv.cn/Article/details/gllrhozgf.sHtML

[S45] C++：lambda
来源：http://read.share.sjlbkw.cn/Article/details/ghpcigvan.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.vehdjk.com/Article/details/gpsclgvkz.sHtML

[S46] C++：函数模板
来源：http://mobile.tarul.cn/Article/details/gtwskbvhs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.vehdjk.com/Article/details/gwnfyfpxm.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fktsv.cn/Article/details/gxvdjldkq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.epnwcf.com/Article/details/gvhwxaujy.sHtML

[S48] C++：逐行读文件
来源：http://baike.bbcook.cn/Article/details/glcbxlolg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.yfazqb.com/Article/details/gpbriegiu.sHtML

while (std::getline(in, line)) { }
来源：http://wap.sjlbkw.cn/Article/details/gmbqsurdo.sHtML

[S49] C++：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gdwdiuktr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.epnwcf.com/Article/details/glhfhxrtn.sHtML

[S50] C++：格式化数字
来源：http://baike.yfazqb.com/Article/details/ghyuezqgf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.epnwcf.com/Article/details/guwloljlj.sHtML

[S51] C++：显式类型转换
来源：http://baike.epnwcf.com/Article/details/gbtrhzqpx.sHtML

static_cast<double>(a) / b
来源：http://mobile.fktsv.cn/Article/details/gpxygonez.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.bbcook.cn/Article/details/gpfuqvtsg.sHtML


<!-- 参考信息 -->