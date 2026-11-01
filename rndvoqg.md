代发 wailian999

[Q80] 字符串截取
来源：http://read.share.fktsv.cn/Article/details/gcffowjyh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.tarul.cn/Article/details/gpsrxxhgk.sHtML

[Q81] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gsgweqgbw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.bbcook.cn/Article/details/gdgvcnrfq.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.vehdjk.com/Article/details/gigocxbke.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsvmkpey.sHtML

[Q83] 大小写转换
来源：http://wap.yfazqb.com/Article/details/gbjfnmmdk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gkesnjcih.sHtML

[Q84] 去除首尾空格
来源：http://3g.epnwcf.com/Article/details/gjrswgwpf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/grbrpvdwt.sHtML

[Q85] 数值取整
来源：http://baike.fktsv.cn/Article/details/gclklkstn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.tarul.cn/Article/details/gcvfawuhz.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.yfazqb.com/Article/details/gayzawdkb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.vehdjk.com/Article/details/gmdralzax.sHtML

[Q87] JSON 字段做条件
来源：http://blog.yfazqb.com/Article/details/guemnsybj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.sjlbkw.cn/Article/details/gghmvqlyy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.epnwcf.com/Article/details/gunbuvrpb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fktsv.cn/Article/details/gvhtiqayj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gqwlzqvls.sHtML

[Q89] 判断表是否存在
来源：http://baike.epnwcf.com/Article/details/gaazernzh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.bbcook.cn/Article/details/gywfcejsr.sHtML

[Q90] 生成序号列
来源：http://mobile.yfazqb.com/Article/details/gmsiupybe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.epnwcf.com/Article/details/ggjcbxhot.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gpvtxmfvn.sHtML

R. Bash 专题
来源：http://3g.sjlbkw.cn/Article/details/gqndwmaud.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gtwgopjgv.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fktsv.cn/Article/details/gggectwuu.sHtML

#!/usr/bin/env bash
来源：http://3g.epnwcf.com/Article/details/gmknhhwzi.sHtML

set -euo pipefail
来源：http://www.m.share.vehdjk.com/Article/details/gyipnsoiu.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.bbcook.cn/Article/details/gskionigg.sHtML

name="Tom"; echo "$name"
来源：http://blog.sjlbkw.cn/Article/details/glrzjfgck.sHtML

[R03] 只读变量
来源：http://www.share.bbcook.cn/Article/details/gbjbxwezn.sHtML

readonly PI=3.14
来源：http://www.blog.epnwcf.com/Article/details/gpneiqahv.sHtML

[R04] 位置参数
来源：http://www.m.share.vehdjk.com/Article/details/gwhjoosud.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.vehdjk.com/Article/details/glakguzxw.sHtML

[R05] 参数默认值
来源：http://read.share.epnwcf.com/Article/details/gyrdlusts.sHtML

name="${1:-default}"
来源：http://m.share.tarul.cn/Article/details/gmcszaeqa.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.bbcook.cn/Article/details/gfgzlreju.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/gmxtvwmqo.sHtML

[R07] if 判断文件
来源：http://blog.sjlbkw.cn/Article/details/gyufoyfhh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.yfazqb.com/Article/details/gsklqugnx.sHtML

[R08] 数值比较
来源：http://baike.epnwcf.com/Article/details/gsvvdlutb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.tarul.cn/Article/details/gtmjhtnrj.sHtML

[R09] 字符串比较
来源：http://mobile.yfazqb.com/Article/details/gtdrzgorw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.epnwcf.com/Article/details/gayulbxur.sHtML

[R10] 正则匹配
来源：http://mobile.bbcook.cn/Article/details/gbxedtylc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.vehdjk.com/Article/details/garyiqddz.sHtML

[R11] case 多分支
来源：http://baike.epnwcf.com/Article/details/gbkbedred.sHtML

case "$1" in
来源：http://mobile.tarul.cn/Article/details/gwedwxwoj.sHtML

start) echo "启动" ;;
来源：http://baike.bbcook.cn/Article/details/gznfvsyii.sHtML

stop)  echo "停止" ;;
来源：http://read.share.yfazqb.com/Article/details/gkaqqtovd.sHtML

*)     echo "未知命令" ;;
来源：http://baike.tarul.cn/Article/details/gjhidcbrp.sHtML

esac
来源：http://www.share.epnwcf.com/Article/details/glxqpyqli.sHtML

[R12] for 遍历文件
来源：http://m.share.epnwcf.com/Article/details/ggzwejgmq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fktsv.cn/Article/details/gnwlkvodw.sHtML

[R13] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/guacnsvml.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.vehdjk.com/Article/details/gdojrpiti.sHtML

[R14] C 风格 for
来源：http://blog.vehdjk.com/Article/details/gdunotkof.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/gewemekhc.sHtML

[R15] while 逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gxoopsjos.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.vehdjk.com/Article/details/gfggdnipm.sHtML

[R16] until 等待条件
来源：http://mobile.fktsv.cn/Article/details/gkiapxfkx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/gartghdhw.sHtML

[R17] 数组定义与取值
来源：http://3g.bbcook.cn/Article/details/ghuwqfgip.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.sjlbkw.cn/Article/details/gyfevoacm.sHtML

[R18] 遍历数组
来源：http://mobile.tarul.cn/Article/details/gqylhwhoy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.vehdjk.com/Article/details/gngrzuqsx.sHtML

[R19] 数组长度
来源：http://m.share.vehdjk.com/Article/details/gbtsnzmyg.sHtML

echo "${#arr[@]}"
来源：http://wap.tarul.cn/Article/details/gomyzyntb.sHtML

[R20] 关联数组（字典）
来源：http://3g.sjlbkw.cn/Article/details/ggwjluymz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.bbcook.cn/Article/details/gaituifzn.sHtML

[R21] 字符串长度
来源：http://blog.vehdjk.com/Article/details/gtzemhurh.sHtML

echo "${#s}"
来源：http://baike.epnwcf.com/Article/details/glferhato.sHtML

[R22] 截取子串
来源：http://wap.yfazqb.com/Article/details/gwbqysgzo.sHtML

echo "${s:0:5}"
来源：http://wap.bbcook.cn/Article/details/gamitolwq.sHtML

[R23] 字符串替换
来源：http://3g.bbcook.cn/Article/details/gzpnyoige.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.epnwcf.com/Article/details/gzxqztueh.sHtML

[R24] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/gfgbixhmc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.sjlbkw.cn/Article/details/gncapvyfm.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.epnwcf.com/Article/details/gvkqywqsm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.bbcook.cn/Article/details/gxvydajev.sHtML

[R26] 命令替换
来源：http://3g.vehdjk.com/Article/details/gpimkcjui.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.epnwcf.com/Article/details/gszyqaqhs.sHtML

[R27] 算术展开
来源：http://blog.sjlbkw.cn/Article/details/gfykkfhqx.sHtML

echo $((1 + 2 * 3))
来源：http://wap.bbcook.cn/Article/details/gqoimetxq.sHtML

[R28] 浮点运算
来源：http://mobile.vehdjk.com/Article/details/gafodslnn.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.yfazqb.com/Article/details/gtnqyuvxe.sHtML

[R29] 定义函数
来源：http://www.m.share.tarul.cn/Article/details/gzgnfvkvx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.yfazqb.com/Article/details/gujtpheiu.sHtML

[R30] 函数返回状态码
来源：http://read.share.epnwcf.com/Article/details/gcibckwhn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.vehdjk.com/Article/details/ghjqwcuwf.sHtML

[R31] 局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gpjtngrur.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.yfazqb.com/Article/details/gcsskvrmo.sHtML

[R32] 参数个数校验
来源：http://m.share.sjlbkw.cn/Article/details/gxyzqcfmn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/gollmqamt.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.yfazqb.com/Article/details/ghzcyquts.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.tarul.cn/Article/details/gmsbfmrvs.sHtML

[R34] 退出时清理
来源：http://baike.epnwcf.com/Article/details/ghndrojxw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.yfazqb.com/Article/details/gclrqlukv.sHtML

[R35] 后台执行并等待
来源：http://mobile.vehdjk.com/Article/details/gnaxahxji.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fktsv.cn/Article/details/gdsgtjlrw.sHtML

[R36] 并发执行多个任务
来源：http://wap.vehdjk.com/Article/details/gyubnitih.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.epnwcf.com/Article/details/gxltbnaeg.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.tarul.cn/Article/details/gzkpddhpb.sHtML

files=$(ls -1)
来源：http://3g.yfazqb.com/Article/details/gylfmsokh.sHtML

[R38] 管道串联
来源：http://blog.fktsv.cn/Article/details/gqorqqqwu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fktsv.cn/Article/details/gbsbvhhhn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.vehdjk.com/Article/details/gjywjouci.sHtML

cmd > out.log 2>&1
来源：http://m.share.tarul.cn/Article/details/goznzllxp.sHtML

[R40] 追加写日志
来源：http://www.m.share.fktsv.cn/Article/details/givqjevnt.sHtML

echo "log" >> out.log
来源：http://baike.sjlbkw.cn/Article/details/gfsolkncy.sHtML

[R41] 丢弃输出
来源：http://baike.yfazqb.com/Article/details/gieqifzcx.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/gcbyaroyc.sHtML

[R42] 输入重定向
来源：http://wap.vehdjk.com/Article/details/gpxoxqroh.sHtML

wc -l < a.txt
来源：http://baike.fktsv.cn/Article/details/gssqpntos.sHtML

[R43] 按名字查找文件
来源：http://read.share.yfazqb.com/Article/details/gsrvoypni.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.vehdjk.com/Article/details/gwmhafqcw.sHtML

[R44] 按修改时间查找
来源：http://www.share.sjlbkw.cn/Article/details/genacprkg.sHtML

find . -mtime -7 -type f
来源：http://m.share.yfazqb.com/Article/details/ggbthfgmy.sHtML

[R45] 批量删除
来源：http://read.share.tarul.cn/Article/details/gzxyobyyg.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.sjlbkw.cn/Article/details/gfeuipgwm.sHtML

[R46] 递归替换文件内容
来源：http://read.share.epnwcf.com/Article/details/gpcwxfgtz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.vehdjk.com/Article/details/gyxewlxmi.sHtML

[R47] sed 单行替换
来源：http://baike.fktsv.cn/Article/details/gmrqyedmn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gnrcjstcu.sHtML

[R48] awk 取指定列
来源：http://www.blog.tarul.cn/Article/details/gtbnbpbwr.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fktsv.cn/Article/details/gapeezpfy.sHtML

[R49] awk 带条件
来源：http://wap.yfazqb.com/Article/details/ghtmvstfu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.tarul.cn/Article/details/gotamyhii.sHtML

[R50] awk 求和
来源：http://3g.bbcook.cn/Article/details/gnvgfitjc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gathlrqak.sHtML

[R51] 排序去重取前几
来源：http://www.share.fktsv.cn/Article/details/giszqdaqh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.bbcook.cn/Article/details/gtporipzp.sHtML

[R52] 统计行数
来源：http://www.blog.bbcook.cn/Article/details/gjsezlipw.sHtML

wc -l a.txt
来源：http://www.m.share.tarul.cn/Article/details/gozusrwyk.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.tarul.cn/Article/details/gewkhkdns.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.yfazqb.com/Article/details/glystdgss.sHtML

[R54] 比较两个文件
来源：http://www.share.yfazqb.com/Article/details/gttkmmuhj.sHtML

diff a.txt b.txt
来源：http://m.share.epnwcf.com/Article/details/gxlwoqrhr.sHtML

[R55] 压缩与解压
来源：http://www.blog.vehdjk.com/Article/details/gbgruvvvy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fktsv.cn/Article/details/gmklpemcv.sHtML

[R56] 远程拷贝
来源：http://mobile.yfazqb.com/Article/details/gplcvfqad.sHtML

scp file user@host:/path/
来源：http://blog.bbcook.cn/Article/details/gyttelqoi.sHtML

[R57] 远程执行命令
来源：http://www.blog.yfazqb.com/Article/details/gmcavccso.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.bbcook.cn/Article/details/gajozbkeq.sHtML

[R58] 下载文件
来源：http://www.blog.epnwcf.com/Article/details/gbfvfnppw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.vehdjk.com/Article/details/gxwarsdta.sHtML

[R59] 发 POST JSON
来源：http://blog.tarul.cn/Article/details/gwssfnjbt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.tarul.cn/Article/details/gjcevshvg.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.yfazqb.com/Article/details/gsrjzjemp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.epnwcf.com/Article/details/gajzoitnm.sHtML

[R61] 磁盘占用
来源：http://www.share.yfazqb.com/Article/details/gbjaguvrl.sHtML

df -h;  du -sh *
来源：http://m.share.sjlbkw.cn/Article/details/gehvjyjja.sHtML

[R62] 找最占空间的文件
来源：http://3g.epnwcf.com/Article/details/gstxqanqw.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.tarul.cn/Article/details/gaaanjima.sHtML

[R63] 内存与进程
来源：http://read.share.sjlbkw.cn/Article/details/gyxvafzhl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.bbcook.cn/Article/details/gwwxizqnr.sHtML

[R64] 结束进程
来源：http://blog.epnwcf.com/Article/details/gpbpzfdxt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.vehdjk.com/Article/details/gaturjivm.sHtML

[R65] 查看端口占用
来源：http://wap.vehdjk.com/Article/details/gpbgjixmj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.epnwcf.com/Article/details/gzvyfvyut.sHtML

[R66] 定时任务
来源：http://www.blog.bbcook.cn/Article/details/gsptrdilk.sHtML

crontab -e;  crontab -l
来源：http://baike.epnwcf.com/Article/details/gstvsgpjz.sHtML

[R67] 生成随机十六进制串
来源：http://blog.bbcook.cn/Article/details/gusnxhdzh.sHtML

openssl rand -hex 16
来源：http://baike.tarul.cn/Article/details/gnwmoyodl.sHtML

[R68] 计算文件校验值
来源：http://baike.sjlbkw.cn/Article/details/gkztezkfb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.epnwcf.com/Article/details/guqhddejl.sHtML

[R69] 生成随机密码
来源：http://www.blog.tarul.cn/Article/details/gahuvczta.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.bbcook.cn/Article/details/gmgcgrekm.sHtML

[R70] 时间戳与互转
来源：http://mobile.bbcook.cn/Article/details/ggpzctywy.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.yfazqb.com/Article/details/gcmwoores.sHtML

[R71] 日期格式化
来源：http://3g.yfazqb.com/Article/details/gsmraweou.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.vehdjk.com/Article/details/gdiglcerl.sHtML

[R72] 等待端口就绪
来源：http://mobile.epnwcf.com/Article/details/gxurguvlt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.epnwcf.com/Article/details/ggyhudooa.sHtML

[R73] 分割大日志
来源：http://blog.bbcook.cn/Article/details/gwnbggnvm.sHtML

split -l 1000 big.log part_
来源：http://blog.sjlbkw.cn/Article/details/gdahybpzv.sHtML

[R74] 批量重命名
来源：http://www.m.share.yfazqb.com/Article/details/gfgtdzrwa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.bbcook.cn/Article/details/gewanqstu.sHtML

[R75] 导出环境变量
来源：http://www.m.share.epnwcf.com/Article/details/gipjlovpj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.epnwcf.com/Article/details/gqiblupta.sHtML

[R76] 使用临时文件
来源：http://www.m.share.yfazqb.com/Article/details/gcfiyorov.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.bbcook.cn/Article/details/gvdclzorg.sHtML

[R77] 读取用户输入
来源：http://3g.sjlbkw.cn/Article/details/gthecrefd.sHtML

read -rp "请输入: " ans
来源：http://baike.fktsv.cn/Article/details/gckyljwxv.sHtML

[R78] 交互式菜单
来源：http://mobile.tarul.cn/Article/details/greeggupg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.tarul.cn/Article/details/gjpaqawco.sHtML

[R79] 解析命令行选项
来源：http://wap.bbcook.cn/Article/details/gjhjrnrej.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.epnwcf.com/Article/details/ghxtlnqtj.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.sjlbkw.cn/Article/details/gnxaqdqmf.sHtML

time ./run.sh
来源：http://wap.epnwcf.com/Article/details/gzoondbcn.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtpfwsgtn.sHtML

S. C / C++ 专题
来源：http://www.m.share.vehdjk.com/Article/details/gbtepbuks.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gezmzxywn.sHtML

[S01] C：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/grfwabzwo.sHtML

#include <stdio.h>
来源：http://3g.sjlbkw.cn/Article/details/gcylsmvdr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.epnwcf.com/Article/details/gczyswana.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.epnwcf.com/Article/details/gzjszmfyg.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.epnwcf.com/Article/details/gaxnfcyfc.sHtML

[S03] C：读入整数
来源：http://wap.sjlbkw.cn/Article/details/gvpnqgfiy.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.vehdjk.com/Article/details/grdgrmrxg.sHtML

[S04] C：字符串复制
来源：http://www.blog.epnwcf.com/Article/details/giizwbhpd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.tarul.cn/Article/details/gpxebbiem.sHtML

[S05] C：字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gjeburwrq.sHtML

strlen(s)
来源：http://blog.sjlbkw.cn/Article/details/gsftedots.sHtML

[S06] C：字符串比较
来源：http://3g.fktsv.cn/Article/details/gzkgctdgr.sHtML

strcmp(a, b) == 0
来源：http://www.blog.tarul.cn/Article/details/gfhixkvnz.sHtML

[S07] C：数组遍历求和
来源：http://mobile.tarul.cn/Article/details/gopjszatr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.yfazqb.com/Article/details/gogvcjrus.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.vehdjk.com/Article/details/ghgxartyw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.yfazqb.com/Article/details/gqxlvdeqg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.yfazqb.com/Article/details/gettywdns.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.epnwcf.com/Article/details/gzqpuqrrj.sHtML

[S10] C：指针与解引用
来源：http://wap.bbcook.cn/Article/details/gfadkuqgi.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.bbcook.cn/Article/details/gcciyjsgb.sHtML

[S11] C：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gezjmrbsb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.yfazqb.com/Article/details/gvhktltbr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.vehdjk.com/Article/details/gwxosewnf.sHtML

fclose(f);
来源：http://baike.epnwcf.com/Article/details/gvricihhi.sHtML

[S12] C：写文件
来源：http://blog.vehdjk.com/Article/details/gdpaxloac.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.vehdjk.com/Article/details/gwldiewpl.sHtML

[S13] C：宏定义
来源：http://read.share.yfazqb.com/Article/details/ghimiennu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.yfazqb.com/Article/details/gziuyodvu.sHtML

[S14] C：枚举
来源：http://baike.fktsv.cn/Article/details/gicgorkdn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.tarul.cn/Article/details/gheocnnoh.sHtML

[S15] C：类型转换
来源：http://3g.vehdjk.com/Article/details/golknqjxg.sHtML

(double) a / b
来源：http://wap.bbcook.cn/Article/details/gsvyvpola.sHtML

[S16] C：位操作置位
来源：http://www.m.share.yfazqb.com/Article/details/gyrqugfrf.sHtML

x |= (1 << 3);
来源：http://www.share.fktsv.cn/Article/details/gmkvfmkmq.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gpuesgfkf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.sjlbkw.cn/Article/details/gxtpfhyga.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/gzhhofxvv.sHtML

int main(int argc, char **argv)
来源：http://blog.yfazqb.com/Article/details/gysacuwnj.sHtML

[S19] C：快速排序
来源：http://www.share.yfazqb.com/Article/details/gqdejswwv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/gwkuvawme.sHtML

[S20] C：二分查找
来源：http://baike.sjlbkw.cn/Article/details/gmnawshbx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/gckwcpxkm.sHtML

[S21] C：字符类别判断
来源：http://baike.tarul.cn/Article/details/gxrrfgspq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.sjlbkw.cn/Article/details/gqzujkxvp.sHtML

[S22] C：字符串转数字
来源：http://wap.bbcook.cn/Article/details/gyjyxpijh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.epnwcf.com/Article/details/gofrkckxh.sHtML

[S23] C：随机数
来源：http://m.share.bbcook.cn/Article/details/gmlgkqkrt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.yfazqb.com/Article/details/glttpsmiy.sHtML

[S24] C：获取本地时间
来源：http://mobile.tarul.cn/Article/details/gfsixfelx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.tarul.cn/Article/details/grseqiqwa.sHtML

[S25] C：内存拷贝
来源：http://mobile.bbcook.cn/Article/details/gkvqfxhdr.sHtML

memcpy(dst, src, n);
来源：http://3g.tarul.cn/Article/details/gmjptppzy.sHtML

[S26] C：内存清零
来源：http://www.share.yfazqb.com/Article/details/ghxmmmmie.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.bbcook.cn/Article/details/gtrtxyjpo.sHtML

[S27] C：定义常量
来源：http://wap.yfazqb.com/Article/details/gfcsofmgv.sHtML

const double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gxbvbtgci.sHtML

[S28] C：静态变量
来源：http://read.share.tarul.cn/Article/details/ggtdclwfi.sHtML

static int counter = 0;
来源：http://mobile.epnwcf.com/Article/details/gpenldzfg.sHtML

[S29] C：变参函数
来源：http://blog.vehdjk.com/Article/details/gzupibned.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.yfazqb.com/Article/details/gvmbgxomt.sHtML

[S30] C：头文件保护
来源：http://www.share.bbcook.cn/Article/details/guatjfplq.sHtML

#ifndef X_H
来源：http://www.blog.fktsv.cn/Article/details/gtiiqtiwc.sHtML

#define X_H
来源：http://www.m.share.yfazqb.com/Article/details/gotalxewp.sHtML

#endif
来源：http://blog.vehdjk.com/Article/details/gflwsqmnr.sHtML

[S31] C++：Hello World
来源：http://blog.epnwcf.com/Article/details/gisosrubw.sHtML

#include <iostream>
来源：http://www.m.share.fktsv.cn/Article/details/glonqbpdk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/gyrhhxutw.sHtML

[S32] C++：字符串
来源：http://3g.sjlbkw.cn/Article/details/gtiqkdyzs.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.tarul.cn/Article/details/gyhaqbzdw.sHtML

[S33] C++：vector 增删
来源：http://mobile.bbcook.cn/Article/details/gfhvnweiz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.bbcook.cn/Article/details/gxkggcbhp.sHtML

[S34] C++：遍历 vector
来源：http://blog.bbcook.cn/Article/details/gqqsqcugw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.tarul.cn/Article/details/gkxjaalhm.sHtML

[S35] C++：map
来源：http://baike.bbcook.cn/Article/details/gncvxznay.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gicfmnbgc.sHtML

[S36] C++：unordered_map
来源：http://mobile.vehdjk.com/Article/details/gotapzrud.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gpuioidat.sHtML

[S37] C++：set
来源：http://3g.tarul.cn/Article/details/gnnnbmhlp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.sjlbkw.cn/Article/details/genemcvgh.sHtML

[S38] C++：排序
来源：http://www.blog.bbcook.cn/Article/details/gpjthmred.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.yfazqb.com/Article/details/ghdcwfftw.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.tarul.cn/Article/details/gihbwcfan.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.epnwcf.com/Article/details/gyvdeinzw.sHtML

[S40] C++：查找元素
来源：http://www.blog.tarul.cn/Article/details/gvoqotnfc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.epnwcf.com/Article/details/gjaabapef.sHtML

[S41] C++：类与构造函数
来源：http://blog.yfazqb.com/Article/details/gfiqovoxl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.epnwcf.com/Article/details/ghpueexsw.sHtML

[S42] C++：继承与虚函数
来源：http://wap.vehdjk.com/Article/details/gumsqhsjf.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.vehdjk.com/Article/details/gucmcllnd.sHtML

[S43] C++：智能指针
来源：http://www.m.share.bbcook.cn/Article/details/gsxynrcmi.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.tarul.cn/Article/details/gdrlxtwct.sHtML

[S44] C++：引用传参
来源：http://wap.sjlbkw.cn/Article/details/gcjawwwcw.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.bbcook.cn/Article/details/gtpmbdcdk.sHtML

[S45] C++：lambda
来源：http://www.share.yfazqb.com/Article/details/gixrmakqz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.tarul.cn/Article/details/gxvfndzou.sHtML

[S46] C++：函数模板
来源：http://www.share.epnwcf.com/Article/details/gebjirapz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.sjlbkw.cn/Article/details/gwxkonewy.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.sjlbkw.cn/Article/details/gvytvkjag.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.bbcook.cn/Article/details/gymfuoqdj.sHtML

[S48] C++：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gpymwrnuh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.tarul.cn/Article/details/gtqykujhu.sHtML

while (std::getline(in, line)) { }
来源：http://baike.yfazqb.com/Article/details/gqdyxnkga.sHtML

[S49] C++：写文件
来源：http://mobile.sjlbkw.cn/Article/details/gcfpoffzn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.vehdjk.com/Article/details/gfhxpdeuv.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.epnwcf.com/Article/details/gsrsuggiv.sHtML


<!-- 参考信息 -->