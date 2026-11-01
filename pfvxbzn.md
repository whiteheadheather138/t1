代发 wailian999

[Q76] 按天统计
来源：http://mobile.bbcook.cn/Article/details/gnmmgdfow.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fktsv.cn/Article/details/gybbsrbqe.sHtML

[Q77] 时间加减
来源：http://www.m.share.tarul.cn/Article/details/guewlpcuj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.yfazqb.com/Article/details/gortyskau.sHtML

[Q78] 当前时间
来源：http://www.share.sjlbkw.cn/Article/details/gogbnfbtb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.vehdjk.com/Article/details/gyamizcux.sHtML

[Q79] 字符串拼接
来源：http://3g.yfazqb.com/Article/details/gasoejxzn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.vehdjk.com/Article/details/gqdqucwbs.sHtML

[Q80] 字符串截取
来源：http://mobile.epnwcf.com/Article/details/gqoexbocw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gresildim.sHtML

[Q81] 字符串替换
来源：http://3g.epnwcf.com/Article/details/gryzjlcho.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gzpeibuhu.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.vehdjk.com/Article/details/gzoclutnm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/goozbnxgo.sHtML

[Q83] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gozgzxjxs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gysgysltt.sHtML

[Q84] 去除首尾空格
来源：http://read.share.tarul.cn/Article/details/gfbfzgwcp.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gzdsjxawe.sHtML

[Q85] 数值取整
来源：http://3g.fktsv.cn/Article/details/gzscbvlgs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.vehdjk.com/Article/details/gjkugkflv.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.vehdjk.com/Article/details/gfwkdafur.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.tarul.cn/Article/details/goguxcubp.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fktsv.cn/Article/details/gqonsrcde.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.tarul.cn/Article/details/gnhokegtd.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.sjlbkw.cn/Article/details/ghjkyjadw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.yfazqb.com/Article/details/gdyjddarq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.vehdjk.com/Article/details/gsndrzrsh.sHtML

[Q89] 判断表是否存在
来源：http://read.share.epnwcf.com/Article/details/giyfajhti.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.tarul.cn/Article/details/gvmjmkept.sHtML

[Q90] 生成序号列
来源：http://baike.bbcook.cn/Article/details/ggxjtlbnb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.sjlbkw.cn/Article/details/graqvuvjw.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gbnafqtyb.sHtML

R. Bash 专题
来源：http://read.share.yfazqb.com/Article/details/gzcexqtru.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gpwrmaxxd.sHtML

[R01] shebang 与严格模式
来源：http://3g.epnwcf.com/Article/details/gtfvuigyk.sHtML

#!/usr/bin/env bash
来源：http://blog.vehdjk.com/Article/details/gbaitutjn.sHtML

set -euo pipefail
来源：http://3g.sjlbkw.cn/Article/details/gntrcymoj.sHtML

[R02] 变量赋值与使用
来源：http://www.share.vehdjk.com/Article/details/glgytvafu.sHtML

name="Tom"; echo "$name"
来源：http://www.share.epnwcf.com/Article/details/gahdigntm.sHtML

[R03] 只读变量
来源：http://www.blog.epnwcf.com/Article/details/gmvvstvac.sHtML

readonly PI=3.14
来源：http://www.m.share.fktsv.cn/Article/details/gbwycritb.sHtML

[R04] 位置参数
来源：http://m.share.vehdjk.com/Article/details/gpkhueccc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.tarul.cn/Article/details/gkhdonyxv.sHtML

[R05] 参数默认值
来源：http://baike.tarul.cn/Article/details/gexnfywks.sHtML

name="${1:-default}"
来源：http://mobile.fktsv.cn/Article/details/gyqnewawp.sHtML

[R06] 判断命令是否存在
来源：http://blog.bbcook.cn/Article/details/grxeaknkr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxonxnuzi.sHtML

[R07] if 判断文件
来源：http://www.blog.yfazqb.com/Article/details/gzhtstpnt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.bbcook.cn/Article/details/gupxuzifa.sHtML

[R08] 数值比较
来源：http://www.blog.tarul.cn/Article/details/gsnwandgk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fktsv.cn/Article/details/gffzmmjdf.sHtML

[R09] 字符串比较
来源：http://mobile.vehdjk.com/Article/details/gunptctwj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.tarul.cn/Article/details/gxjczqtcw.sHtML

[R10] 正则匹配
来源：http://3g.yfazqb.com/Article/details/gykkppvyc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.tarul.cn/Article/details/goiwhbtys.sHtML

[R11] case 多分支
来源：http://www.share.yfazqb.com/Article/details/givvtprtz.sHtML

case "$1" in
来源：http://3g.yfazqb.com/Article/details/gqxxedfmu.sHtML

start) echo "启动" ;;
来源：http://baike.epnwcf.com/Article/details/gycpqeyci.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gsmoajvlu.sHtML

*)     echo "未知命令" ;;
来源：http://wap.sjlbkw.cn/Article/details/grtqouvfc.sHtML

esac
来源：http://wap.sjlbkw.cn/Article/details/gdsvhbanv.sHtML

[R12] for 遍历文件
来源：http://wap.vehdjk.com/Article/details/gbsaojkhn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.yfazqb.com/Article/details/gtbfnbtdv.sHtML

[R13] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/glohsxalv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.yfazqb.com/Article/details/gezglktvv.sHtML

[R14] C 风格 for
来源：http://www.blog.bbcook.cn/Article/details/gnkehtsxs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fktsv.cn/Article/details/gjqsibwes.sHtML

[R15] while 逐行读文件
来源：http://wap.yfazqb.com/Article/details/gulsjabgt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.vehdjk.com/Article/details/gvlhftwpo.sHtML

[R16] until 等待条件
来源：http://3g.fktsv.cn/Article/details/gwghkuvsz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.yfazqb.com/Article/details/gaktvdgit.sHtML

[R17] 数组定义与取值
来源：http://blog.vehdjk.com/Article/details/gflnvuqjf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.bbcook.cn/Article/details/gcfhcdaac.sHtML

[R18] 遍历数组
来源：http://www.share.tarul.cn/Article/details/ghadixept.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.vehdjk.com/Article/details/guzgoceyd.sHtML

[R19] 数组长度
来源：http://blog.tarul.cn/Article/details/gfauheesr.sHtML

echo "${#arr[@]}"
来源：http://mobile.epnwcf.com/Article/details/gdribktsn.sHtML

[R20] 关联数组（字典）
来源：http://baike.yfazqb.com/Article/details/gwflxmhrd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fktsv.cn/Article/details/gbiozgpgy.sHtML

[R21] 字符串长度
来源：http://blog.epnwcf.com/Article/details/gujeuuabv.sHtML

echo "${#s}"
来源：http://www.m.share.yfazqb.com/Article/details/gvmlhfaqg.sHtML

[R22] 截取子串
来源：http://blog.tarul.cn/Article/details/gasnjsjzm.sHtML

echo "${s:0:5}"
来源：http://mobile.yfazqb.com/Article/details/gvkwziaxj.sHtML

[R23] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/gilloqaoq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.yfazqb.com/Article/details/gxpkwjqdl.sHtML

[R24] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/gmlockduv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.epnwcf.com/Article/details/gtowhncsg.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fktsv.cn/Article/details/gtsxjhzqg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.vehdjk.com/Article/details/gxnpjohzn.sHtML

[R26] 命令替换
来源：http://www.share.sjlbkw.cn/Article/details/gakndumhj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.tarul.cn/Article/details/gjhaiwtgo.sHtML

[R27] 算术展开
来源：http://baike.sjlbkw.cn/Article/details/glggadkfp.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fktsv.cn/Article/details/gmnyemnyk.sHtML

[R28] 浮点运算
来源：http://3g.sjlbkw.cn/Article/details/gtwgfiqhh.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.bbcook.cn/Article/details/glzskwalg.sHtML

[R29] 定义函数
来源：http://m.share.fktsv.cn/Article/details/gisaxtcmz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.vehdjk.com/Article/details/gphknmqco.sHtML

[R30] 函数返回状态码
来源：http://wap.tarul.cn/Article/details/gpgwwhywf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.vehdjk.com/Article/details/gmahcqkds.sHtML

[R31] 局部变量
来源：http://read.share.yfazqb.com/Article/details/gxccmfekc.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.vehdjk.com/Article/details/gtasudgaa.sHtML

[R32] 参数个数校验
来源：http://wap.bbcook.cn/Article/details/gvbzqvfgk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gahmecgcf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.sjlbkw.cn/Article/details/gixjeuuxv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.sjlbkw.cn/Article/details/gcywezkvu.sHtML

[R34] 退出时清理
来源：http://www.blog.tarul.cn/Article/details/guxtsarej.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.sjlbkw.cn/Article/details/gzitexkqs.sHtML

[R35] 后台执行并等待
来源：http://3g.bbcook.cn/Article/details/glcbjwzaq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/gpoomvjpq.sHtML

[R36] 并发执行多个任务
来源：http://mobile.vehdjk.com/Article/details/gxgwhvrui.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.epnwcf.com/Article/details/gfucrzmfs.sHtML

[R37] 把输出赋给变量
来源：http://mobile.yfazqb.com/Article/details/ggkyfhwcc.sHtML

files=$(ls -1)
来源：http://m.share.sjlbkw.cn/Article/details/gadvnlvhw.sHtML

[R38] 管道串联
来源：http://wap.yfazqb.com/Article/details/ghepzsmor.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.tarul.cn/Article/details/gutuynwol.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.sjlbkw.cn/Article/details/gmfshmucy.sHtML

cmd > out.log 2>&1
来源：http://read.share.tarul.cn/Article/details/gorcbvkyw.sHtML

[R40] 追加写日志
来源：http://wap.bbcook.cn/Article/details/ggkuvsbno.sHtML

echo "log" >> out.log
来源：http://wap.yfazqb.com/Article/details/gpdvxafxk.sHtML

[R41] 丢弃输出
来源：http://m.share.vehdjk.com/Article/details/gldsrhpfg.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.bbcook.cn/Article/details/gkeciarvi.sHtML

[R42] 输入重定向
来源：http://m.share.sjlbkw.cn/Article/details/ghpfsxutv.sHtML

wc -l < a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gzztlrpmj.sHtML

[R43] 按名字查找文件
来源：http://3g.bbcook.cn/Article/details/gnexxlwuu.sHtML

find . -name "*.log" -type f
来源：http://read.share.tarul.cn/Article/details/gfaueoeay.sHtML

[R44] 按修改时间查找
来源：http://blog.vehdjk.com/Article/details/ghiorqtqz.sHtML

find . -mtime -7 -type f
来源：http://www.share.bbcook.cn/Article/details/gbpbqbgtb.sHtML

[R45] 批量删除
来源：http://www.m.share.sjlbkw.cn/Article/details/glouhjjqm.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.epnwcf.com/Article/details/glrhmobjs.sHtML

[R46] 递归替换文件内容
来源：http://blog.tarul.cn/Article/details/gobasvbvd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.vehdjk.com/Article/details/gpekdbztp.sHtML

[R47] sed 单行替换
来源：http://read.share.sjlbkw.cn/Article/details/gxczookqu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fktsv.cn/Article/details/gcqurgdqb.sHtML

[R48] awk 取指定列
来源：http://read.share.tarul.cn/Article/details/glowejjdv.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fktsv.cn/Article/details/grlqbjvpd.sHtML

[R49] awk 带条件
来源：http://3g.fktsv.cn/Article/details/ggszeswid.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.tarul.cn/Article/details/gpobczxta.sHtML

[R50] awk 求和
来源：http://blog.sjlbkw.cn/Article/details/gkgtctpyr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gjcvbbwuo.sHtML

[R51] 排序去重取前几
来源：http://www.share.sjlbkw.cn/Article/details/gmcglzyvi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.epnwcf.com/Article/details/gknxqthzf.sHtML

[R52] 统计行数
来源：http://www.blog.bbcook.cn/Article/details/golotepcf.sHtML

wc -l a.txt
来源：http://wap.yfazqb.com/Article/details/gfztesfxt.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.epnwcf.com/Article/details/gvucalsbr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.yfazqb.com/Article/details/gmaactved.sHtML

[R54] 比较两个文件
来源：http://read.share.fktsv.cn/Article/details/gfweiuanm.sHtML

diff a.txt b.txt
来源：http://www.blog.bbcook.cn/Article/details/gwhlaneni.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fktsv.cn/Article/details/gxbehdkjm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.vehdjk.com/Article/details/gsawkaquv.sHtML

[R56] 远程拷贝
来源：http://baike.bbcook.cn/Article/details/gelceysxb.sHtML

scp file user@host:/path/
来源：http://baike.vehdjk.com/Article/details/giyqvpjye.sHtML

[R57] 远程执行命令
来源：http://mobile.bbcook.cn/Article/details/guuaeggjj.sHtML

ssh user@host 'uptime'
来源：http://blog.vehdjk.com/Article/details/gsonsuflb.sHtML

[R58] 下载文件
来源：http://baike.sjlbkw.cn/Article/details/gjepvuznj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.epnwcf.com/Article/details/gomscvqnx.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fktsv.cn/Article/details/gbolnvxmd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.tarul.cn/Article/details/gejxkzxtk.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.tarul.cn/Article/details/guhgtazln.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.yfazqb.com/Article/details/gdbrhoiig.sHtML

[R61] 磁盘占用
来源：http://www.blog.tarul.cn/Article/details/gpmklpqbg.sHtML

df -h;  du -sh *
来源：http://baike.fktsv.cn/Article/details/gxkischhx.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.bbcook.cn/Article/details/gkjkqtzyn.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.yfazqb.com/Article/details/giumklgmm.sHtML

[R63] 内存与进程
来源：http://wap.bbcook.cn/Article/details/ggxvtqoqv.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.epnwcf.com/Article/details/gfwccrljp.sHtML

[R64] 结束进程
来源：http://www.share.epnwcf.com/Article/details/givxfdbev.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.bbcook.cn/Article/details/ghsdsvaeq.sHtML

[R65] 查看端口占用
来源：http://blog.vehdjk.com/Article/details/glcptneyj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.bbcook.cn/Article/details/grkuxofyg.sHtML

[R66] 定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/gnhqgwtln.sHtML

crontab -e;  crontab -l
来源：http://blog.bbcook.cn/Article/details/gfeoyqdhv.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.tarul.cn/Article/details/glkzucyrg.sHtML

openssl rand -hex 16
来源：http://3g.fktsv.cn/Article/details/guslyqnas.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.epnwcf.com/Article/details/grxbapdos.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.yfazqb.com/Article/details/gkqqdzpaz.sHtML

[R69] 生成随机密码
来源：http://www.share.bbcook.cn/Article/details/gzunqcxxa.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.vehdjk.com/Article/details/gtofwuenw.sHtML

[R70] 时间戳与互转
来源：http://www.blog.tarul.cn/Article/details/gcpngiyld.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.bbcook.cn/Article/details/gzngnspkn.sHtML

[R71] 日期格式化
来源：http://mobile.yfazqb.com/Article/details/gppziexny.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.bbcook.cn/Article/details/gcklwxxys.sHtML

[R72] 等待端口就绪
来源：http://mobile.vehdjk.com/Article/details/ggbfdamxb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/gdukwqflu.sHtML

[R73] 分割大日志
来源：http://www.share.sjlbkw.cn/Article/details/gnqztyqan.sHtML

split -l 1000 big.log part_
来源：http://read.share.vehdjk.com/Article/details/grwzycgra.sHtML

[R74] 批量重命名
来源：http://read.share.fktsv.cn/Article/details/gtkifqplm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.bbcook.cn/Article/details/gfrpiiioq.sHtML

[R75] 导出环境变量
来源：http://www.share.fktsv.cn/Article/details/grsmkgytr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.yfazqb.com/Article/details/guxhfmvlu.sHtML

[R76] 使用临时文件
来源：http://www.blog.bbcook.cn/Article/details/gsxhqtqpz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/ghfcrzkub.sHtML

[R77] 读取用户输入
来源：http://m.share.bbcook.cn/Article/details/ghqkkivmm.sHtML

read -rp "请输入: " ans
来源：http://read.share.yfazqb.com/Article/details/gittsgaiq.sHtML

[R78] 交互式菜单
来源：http://www.share.fktsv.cn/Article/details/gaxyxubmf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.tarul.cn/Article/details/gigyogiit.sHtML

[R79] 解析命令行选项
来源：http://m.share.fktsv.cn/Article/details/gsvpkndeq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.tarul.cn/Article/details/gtarhxxhc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.bbcook.cn/Article/details/grdntrerv.sHtML

time ./run.sh
来源：http://www.m.share.fktsv.cn/Article/details/gjqoahqcp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gcwnftflx.sHtML

S. C / C++ 专题
来源：http://read.share.bbcook.cn/Article/details/gdkdyitds.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gxktdsjne.sHtML

[S01] C：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gapmmxuut.sHtML

#include <stdio.h>
来源：http://3g.epnwcf.com/Article/details/gnqzloyjv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.sjlbkw.cn/Article/details/guoqlctqv.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.vehdjk.com/Article/details/gighmagvi.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.vehdjk.com/Article/details/gyjkiexco.sHtML

[S03] C：读入整数
来源：http://www.share.tarul.cn/Article/details/geyfstyfw.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.vehdjk.com/Article/details/getwzqyqt.sHtML

[S04] C：字符串复制
来源：http://3g.bbcook.cn/Article/details/gdehyxman.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.tarul.cn/Article/details/gqwiiqcmv.sHtML

[S05] C：字符串长度
来源：http://read.share.fktsv.cn/Article/details/gtekychwj.sHtML

strlen(s)
来源：http://m.share.fktsv.cn/Article/details/gmvzdwmsz.sHtML

[S06] C：字符串比较
来源：http://baike.vehdjk.com/Article/details/gcespocyu.sHtML

strcmp(a, b) == 0
来源：http://read.share.vehdjk.com/Article/details/gtynxtrwg.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.vehdjk.com/Article/details/gjbjhlktq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.yfazqb.com/Article/details/gappeyoih.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.bbcook.cn/Article/details/gjqxnwime.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.sjlbkw.cn/Article/details/gjxqmpjeb.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.epnwcf.com/Article/details/gqffyejeu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.tarul.cn/Article/details/gvadhsxsa.sHtML

[S10] C：指针与解引用
来源：http://wap.yfazqb.com/Article/details/gbqjyjlez.sHtML

int *p = &a;  *p = 5;
来源：http://baike.vehdjk.com/Article/details/gyhhwfphy.sHtML

[S11] C：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gshevexrz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.sjlbkw.cn/Article/details/gkginwdav.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.epnwcf.com/Article/details/grfzptime.sHtML

fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/gdvpsusdj.sHtML

[S12] C：写文件
来源：http://read.share.vehdjk.com/Article/details/guzglvgxa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.yfazqb.com/Article/details/gggueugig.sHtML

[S13] C：宏定义
来源：http://www.share.sjlbkw.cn/Article/details/gxgwlrhpv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.bbcook.cn/Article/details/galipmhfy.sHtML

[S14] C：枚举
来源：http://wap.fktsv.cn/Article/details/gnspdyzdu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.tarul.cn/Article/details/gfpjlsuvi.sHtML

[S15] C：类型转换
来源：http://www.share.epnwcf.com/Article/details/gqqtnrgbu.sHtML

(double) a / b
来源：http://www.blog.vehdjk.com/Article/details/gpucnkmmj.sHtML

[S16] C：位操作置位
来源：http://wap.epnwcf.com/Article/details/gvrzypsau.sHtML

x |= (1 << 3);
来源：http://mobile.yfazqb.com/Article/details/guehrcajx.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/guatnipfx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.yfazqb.com/Article/details/ggxixcytn.sHtML

[S18] C：命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/gydxsyphf.sHtML

int main(int argc, char **argv)
来源：http://read.share.sjlbkw.cn/Article/details/gzvhnvwmi.sHtML

[S19] C：快速排序
来源：http://3g.vehdjk.com/Article/details/gzsbxnipr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/gzqrtukdm.sHtML

[S20] C：二分查找
来源：http://www.m.share.yfazqb.com/Article/details/gaekfykgm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gdthggoad.sHtML

[S21] C：字符类别判断
来源：http://blog.vehdjk.com/Article/details/gbmyhvrbp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.epnwcf.com/Article/details/guiqtrddu.sHtML

[S22] C：字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/gbjgdxwas.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.epnwcf.com/Article/details/gtdhpkflf.sHtML

[S23] C：随机数
来源：http://blog.sjlbkw.cn/Article/details/gchdztche.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.epnwcf.com/Article/details/grgahimkb.sHtML

[S24] C：获取本地时间
来源：http://read.share.tarul.cn/Article/details/gyjkqjphe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.yfazqb.com/Article/details/gotqyaung.sHtML

[S25] C：内存拷贝
来源：http://3g.epnwcf.com/Article/details/gyzlbrlid.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/ggwvvgrda.sHtML

[S26] C：内存清零
来源：http://blog.vehdjk.com/Article/details/gmypieomo.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.bbcook.cn/Article/details/gzmcixlaz.sHtML

[S27] C：定义常量
来源：http://www.share.tarul.cn/Article/details/gswxyqdjm.sHtML

const double PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gmkpoiwqj.sHtML

[S28] C：静态变量
来源：http://blog.fktsv.cn/Article/details/gdbbsuhga.sHtML

static int counter = 0;
来源：http://www.m.share.yfazqb.com/Article/details/guorqxwgu.sHtML

[S29] C：变参函数
来源：http://read.share.sjlbkw.cn/Article/details/gcjggjgrj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.tarul.cn/Article/details/gjxkaqffj.sHtML

[S30] C：头文件保护
来源：http://read.share.sjlbkw.cn/Article/details/gmqvnclho.sHtML

#ifndef X_H
来源：http://mobile.sjlbkw.cn/Article/details/gyvqmbtty.sHtML

#define X_H
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdtpzxvl.sHtML

#endif
来源：http://mobile.yfazqb.com/Article/details/ghvmzzyed.sHtML

[S31] C++：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gxnikqgup.sHtML

#include <iostream>
来源：http://3g.fktsv.cn/Article/details/godotlbgs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.tarul.cn/Article/details/gwswrvcko.sHtML

[S32] C++：字符串
来源：http://blog.tarul.cn/Article/details/gddzhtkcb.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.yfazqb.com/Article/details/gtzpqxrgr.sHtML

[S33] C++：vector 增删
来源：http://www.share.tarul.cn/Article/details/gdpyzykks.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.tarul.cn/Article/details/guomipreq.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.yfazqb.com/Article/details/gtbbpwnjq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/ggxhfsach.sHtML

[S35] C++：map
来源：http://read.share.sjlbkw.cn/Article/details/gxzwqyenl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gdtndhgsg.sHtML

[S36] C++：unordered_map
来源：http://www.blog.bbcook.cn/Article/details/gfsynaaxb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gireenfys.sHtML

[S37] C++：set
来源：http://read.share.bbcook.cn/Article/details/gtubfnrci.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.vehdjk.com/Article/details/gqtorrsbj.sHtML

[S38] C++：排序
来源：http://m.share.vehdjk.com/Article/details/gqvkcdvvi.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fktsv.cn/Article/details/gbhscwnid.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.yfazqb.com/Article/details/gjnpqeavw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.epnwcf.com/Article/details/gkqeokymx.sHtML

[S40] C++：查找元素
来源：http://m.share.tarul.cn/Article/details/gxgodqcbq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fktsv.cn/Article/details/gzdocmxww.sHtML

[S41] C++：类与构造函数
来源：http://wap.sjlbkw.cn/Article/details/goxgvxzro.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.tarul.cn/Article/details/gxotocyku.sHtML

[S42] C++：继承与虚函数
来源：http://3g.yfazqb.com/Article/details/gzppxrgho.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.vehdjk.com/Article/details/ggphrigok.sHtML

[S43] C++：智能指针
来源：http://www.m.share.yfazqb.com/Article/details/gspmfiuww.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.yfazqb.com/Article/details/gremctuck.sHtML

[S44] C++：引用传参
来源：http://wap.bbcook.cn/Article/details/ggbnblqmv.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.sjlbkw.cn/Article/details/gdqcgmqst.sHtML

[S45] C++：lambda
来源：http://www.share.vehdjk.com/Article/details/gdqcaynrx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.tarul.cn/Article/details/gjugksjbn.sHtML

[S46] C++：函数模板
来源：http://wap.vehdjk.com/Article/details/gmrzhefun.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.epnwcf.com/Article/details/gyfdggrfi.sHtML


<!-- 参考信息 -->