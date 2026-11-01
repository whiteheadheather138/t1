代发 wailian999

[Q67] 设置隔离级别
来源：http://baike.bbcook.cn/Article/details/gulokcvoa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.epnwcf.com/Article/details/giqwbsgfs.sHtML

[Q68] 保存点
来源：http://www.share.fktsv.cn/Article/details/gyhreraqa.sHtML

SAVEPOINT sp1;
来源：http://www.share.tarul.cn/Article/details/gmeofunmo.sHtML

ROLLBACK TO sp1;
来源：http://3g.sjlbkw.cn/Article/details/gibcpacos.sHtML

[Q69] 查看执行计划
来源：http://baike.epnwcf.com/Article/details/ghukovini.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.tarul.cn/Article/details/gtemmekzz.sHtML

[Q70] 更新统计信息
来源：http://m.share.yfazqb.com/Article/details/gbevkbwyp.sHtML

ANALYZE TABLE users;
来源：http://blog.fktsv.cn/Article/details/grhnikgby.sHtML

[Q71] 查看建表语句
来源：http://3g.sjlbkw.cn/Article/details/gpqljwwfi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.bbcook.cn/Article/details/gzvizjzsf.sHtML

[Q72] 查看索引
来源：http://read.share.bbcook.cn/Article/details/gcqbnrcre.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fktsv.cn/Article/details/gswbqmqae.sHtML

[Q73] 查看表状态
来源：http://www.blog.vehdjk.com/Article/details/giujlfapc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.epnwcf.com/Article/details/gdvrctyhh.sHtML

[Q74] 强制使用索引
来源：http://mobile.bbcook.cn/Article/details/gggmhovhi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.bbcook.cn/Article/details/gadfddwdg.sHtML

[Q75] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/gomyvxcke.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gklwifpfu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.yfazqb.com/Article/details/gzvwtliwg.sHtML

[Q76] 按天统计
来源：http://m.share.sjlbkw.cn/Article/details/gwjvfxgbe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.tarul.cn/Article/details/gagknlxnp.sHtML

[Q77] 时间加减
来源：http://www.m.share.bbcook.cn/Article/details/gxmveeszb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.yfazqb.com/Article/details/glvqndfrh.sHtML

[Q78] 当前时间
来源：http://wap.epnwcf.com/Article/details/ghazzxqlm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.tarul.cn/Article/details/ghsdzvhbu.sHtML

[Q79] 字符串拼接
来源：http://3g.epnwcf.com/Article/details/glfjdjazm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.epnwcf.com/Article/details/glhooarnw.sHtML

[Q80] 字符串截取
来源：http://3g.bbcook.cn/Article/details/ggrdwvybi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.tarul.cn/Article/details/gzeudvdlb.sHtML

[Q81] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/gwvwmlaof.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.sjlbkw.cn/Article/details/ghrcbgcfh.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.yfazqb.com/Article/details/gzpogkfom.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gasybhwlf.sHtML

[Q83] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gdterxhnk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gaiwbhacu.sHtML

[Q84] 去除首尾空格
来源：http://m.share.sjlbkw.cn/Article/details/gkjwjrudt.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/goacfipoz.sHtML

[Q85] 数值取整
来源：http://m.share.fktsv.cn/Article/details/grpqmjqcv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.tarul.cn/Article/details/gvoaemmdv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmmlkbwn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/gjmtpzbqi.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.vehdjk.com/Article/details/gwesbinar.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.bbcook.cn/Article/details/gywadchma.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fktsv.cn/Article/details/gdlqjogwm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.yfazqb.com/Article/details/gxekrzkxf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.tarul.cn/Article/details/gviupfyue.sHtML

[Q89] 判断表是否存在
来源：http://mobile.yfazqb.com/Article/details/gsfdisrda.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.vehdjk.com/Article/details/gyhvrlapk.sHtML

[Q90] 生成序号列
来源：http://wap.sjlbkw.cn/Article/details/gjgpuerwj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.yfazqb.com/Article/details/guolowrjq.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gfectoowx.sHtML

R. Bash 专题
来源：http://blog.fktsv.cn/Article/details/gzhxrupnk.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/grgypsvyl.sHtML

[R01] shebang 与严格模式
来源：http://3g.tarul.cn/Article/details/giqsyhdmz.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.epnwcf.com/Article/details/gszjdzizk.sHtML

set -euo pipefail
来源：http://wap.bbcook.cn/Article/details/gsesoxjqm.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.epnwcf.com/Article/details/gmqexkedp.sHtML

name="Tom"; echo "$name"
来源：http://read.share.sjlbkw.cn/Article/details/ggqjliyjp.sHtML

[R03] 只读变量
来源：http://3g.yfazqb.com/Article/details/gtvzgxoen.sHtML

readonly PI=3.14
来源：http://wap.bbcook.cn/Article/details/gxelxgzto.sHtML

[R04] 位置参数
来源：http://3g.epnwcf.com/Article/details/gabkaobrb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.tarul.cn/Article/details/gtmgmbitr.sHtML

[R05] 参数默认值
来源：http://blog.bbcook.cn/Article/details/gdqqqlsfn.sHtML

name="${1:-default}"
来源：http://www.m.share.epnwcf.com/Article/details/gomwuwuyy.sHtML

[R06] 判断命令是否存在
来源：http://baike.yfazqb.com/Article/details/gngpndtck.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/gffnfraww.sHtML

[R07] if 判断文件
来源：http://baike.fktsv.cn/Article/details/gotiwmmic.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fktsv.cn/Article/details/gcdxabkxr.sHtML

[R08] 数值比较
来源：http://www.m.share.yfazqb.com/Article/details/gsemjtwdb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.bbcook.cn/Article/details/gtadwakrm.sHtML

[R09] 字符串比较
来源：http://3g.vehdjk.com/Article/details/gflzfhmnr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.yfazqb.com/Article/details/gcoewuxqs.sHtML

[R10] 正则匹配
来源：http://wap.epnwcf.com/Article/details/gvhrbrbtr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.yfazqb.com/Article/details/gcjpzocef.sHtML

[R11] case 多分支
来源：http://wap.epnwcf.com/Article/details/gtsqfzmoy.sHtML

case "$1" in
来源：http://baike.yfazqb.com/Article/details/gerbhfvld.sHtML

start) echo "启动" ;;
来源：http://m.share.fktsv.cn/Article/details/grvmvsyma.sHtML

stop)  echo "停止" ;;
来源：http://m.share.tarul.cn/Article/details/grvsuxsna.sHtML

*)     echo "未知命令" ;;
来源：http://wap.sjlbkw.cn/Article/details/gdpzhhroi.sHtML

esac
来源：http://www.m.share.bbcook.cn/Article/details/gecmadzvg.sHtML

[R12] for 遍历文件
来源：http://mobile.sjlbkw.cn/Article/details/grgkephsa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.epnwcf.com/Article/details/gfmljqino.sHtML

[R13] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gewlpwjsd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.epnwcf.com/Article/details/gfjjdthko.sHtML

[R14] C 风格 for
来源：http://www.blog.vehdjk.com/Article/details/gwuuezyok.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/geyjeajlh.sHtML

[R15] while 逐行读文件
来源：http://mobile.tarul.cn/Article/details/gebeqtpdr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fktsv.cn/Article/details/gursvyacr.sHtML

[R16] until 等待条件
来源：http://www.share.bbcook.cn/Article/details/gnalerxql.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/gvpksypby.sHtML

[R17] 数组定义与取值
来源：http://www.blog.vehdjk.com/Article/details/gcgfdkujp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.tarul.cn/Article/details/gngbedacx.sHtML

[R18] 遍历数组
来源：http://www.m.share.vehdjk.com/Article/details/gkyintxjo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.tarul.cn/Article/details/gytmzuhmi.sHtML

[R19] 数组长度
来源：http://www.m.share.yfazqb.com/Article/details/gpralbkbg.sHtML

echo "${#arr[@]}"
来源：http://read.share.tarul.cn/Article/details/gyxntofid.sHtML

[R20] 关联数组（字典）
来源：http://www.share.epnwcf.com/Article/details/gvgltnzcg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.vehdjk.com/Article/details/gbbirquzh.sHtML

[R21] 字符串长度
来源：http://mobile.tarul.cn/Article/details/gquwgqiwp.sHtML

echo "${#s}"
来源：http://m.share.bbcook.cn/Article/details/gbyjnorad.sHtML

[R22] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/gzllianrj.sHtML

echo "${s:0:5}"
来源：http://3g.vehdjk.com/Article/details/grfrgwotd.sHtML

[R23] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/gwwvjlzpj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.epnwcf.com/Article/details/gkdzrgprn.sHtML

[R24] 大小写转换
来源：http://mobile.epnwcf.com/Article/details/gsmaujvra.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.vehdjk.com/Article/details/glhrmqvwv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.yfazqb.com/Article/details/ggsbfnifn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.tarul.cn/Article/details/gthybnovd.sHtML

[R26] 命令替换
来源：http://wap.sjlbkw.cn/Article/details/gkrddnpxf.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.vehdjk.com/Article/details/gawcsaydg.sHtML

[R27] 算术展开
来源：http://mobile.sjlbkw.cn/Article/details/gjlrqtniz.sHtML

echo $((1 + 2 * 3))
来源：http://baike.yfazqb.com/Article/details/guolimktc.sHtML

[R28] 浮点运算
来源：http://baike.yfazqb.com/Article/details/goreyenra.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.vehdjk.com/Article/details/gycwgklmr.sHtML

[R29] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/gfqwjhxkv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.epnwcf.com/Article/details/gfffhtazq.sHtML

[R30] 函数返回状态码
来源：http://m.share.fktsv.cn/Article/details/goaqfyxff.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.yfazqb.com/Article/details/gvxicaona.sHtML

[R31] 局部变量
来源：http://baike.bbcook.cn/Article/details/gihpbazxo.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.tarul.cn/Article/details/ggpyagmhr.sHtML

[R32] 参数个数校验
来源：http://www.m.share.vehdjk.com/Article/details/gowvvqwqh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/guauocbwr.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fktsv.cn/Article/details/gmdrfpjkl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.vehdjk.com/Article/details/gbilinsie.sHtML

[R34] 退出时清理
来源：http://blog.sjlbkw.cn/Article/details/gvxiqflcb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fktsv.cn/Article/details/gonrrpgqt.sHtML

[R35] 后台执行并等待
来源：http://read.share.tarul.cn/Article/details/gexnnavof.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.yfazqb.com/Article/details/gyqrwwmws.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fktsv.cn/Article/details/gfkrgxbgs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.epnwcf.com/Article/details/guaaulfih.sHtML

[R37] 把输出赋给变量
来源：http://3g.fktsv.cn/Article/details/gywhbxzht.sHtML

files=$(ls -1)
来源：http://read.share.bbcook.cn/Article/details/gwkxtiuib.sHtML

[R38] 管道串联
来源：http://read.share.sjlbkw.cn/Article/details/gerazggpd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.bbcook.cn/Article/details/glpmpcnyw.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.tarul.cn/Article/details/gugulbhei.sHtML

cmd > out.log 2>&1
来源：http://www.share.tarul.cn/Article/details/gcvrjgaid.sHtML

[R40] 追加写日志
来源：http://www.m.share.yfazqb.com/Article/details/gxdqmzxfe.sHtML

echo "log" >> out.log
来源：http://wap.sjlbkw.cn/Article/details/gvmunqtem.sHtML

[R41] 丢弃输出
来源：http://www.share.yfazqb.com/Article/details/gictydkbs.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fktsv.cn/Article/details/gojknsewd.sHtML

[R42] 输入重定向
来源：http://www.m.share.bbcook.cn/Article/details/gjuizaqvv.sHtML

wc -l < a.txt
来源：http://read.share.tarul.cn/Article/details/ghnhywrud.sHtML

[R43] 按名字查找文件
来源：http://m.share.bbcook.cn/Article/details/gadzdosqw.sHtML

find . -name "*.log" -type f
来源：http://mobile.bbcook.cn/Article/details/gwzxzeurz.sHtML

[R44] 按修改时间查找
来源：http://read.share.yfazqb.com/Article/details/gjokythdq.sHtML

find . -mtime -7 -type f
来源：http://wap.tarul.cn/Article/details/gnugzlzhh.sHtML

[R45] 批量删除
来源：http://mobile.bbcook.cn/Article/details/gyipqshzr.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.yfazqb.com/Article/details/gthyknktu.sHtML

[R46] 递归替换文件内容
来源：http://wap.yfazqb.com/Article/details/ghzggcoug.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.sjlbkw.cn/Article/details/gvgtcoquq.sHtML

[R47] sed 单行替换
来源：http://www.share.vehdjk.com/Article/details/gmlocpiio.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.sjlbkw.cn/Article/details/goctbtddv.sHtML

[R48] awk 取指定列
来源：http://www.share.yfazqb.com/Article/details/gedidpuao.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.bbcook.cn/Article/details/gxzvimgaz.sHtML

[R49] awk 带条件
来源：http://www.blog.fktsv.cn/Article/details/gbipfpulr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.tarul.cn/Article/details/gzydwudks.sHtML

[R50] awk 求和
来源：http://blog.fktsv.cn/Article/details/gmoiieiqh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.yfazqb.com/Article/details/ggkqrijlu.sHtML

[R51] 排序去重取前几
来源：http://mobile.vehdjk.com/Article/details/gwjmpatxc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.bbcook.cn/Article/details/goxlezqbn.sHtML

[R52] 统计行数
来源：http://www.blog.tarul.cn/Article/details/gygiwahzd.sHtML

wc -l a.txt
来源：http://blog.sjlbkw.cn/Article/details/gifomedtc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.sjlbkw.cn/Article/details/gdbdjmhjg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.tarul.cn/Article/details/gcpsvswuc.sHtML

[R54] 比较两个文件
来源：http://3g.fktsv.cn/Article/details/gsrdcvwhj.sHtML

diff a.txt b.txt
来源：http://read.share.bbcook.cn/Article/details/gzwlmgzjd.sHtML

[R55] 压缩与解压
来源：http://mobile.bbcook.cn/Article/details/gkkgkrtmq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.bbcook.cn/Article/details/gymquuzqr.sHtML

[R56] 远程拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gvztpjzpn.sHtML

scp file user@host:/path/
来源：http://read.share.tarul.cn/Article/details/gnyzwssiz.sHtML

[R57] 远程执行命令
来源：http://blog.yfazqb.com/Article/details/gtvhimval.sHtML

ssh user@host 'uptime'
来源：http://wap.fktsv.cn/Article/details/glamnpgzn.sHtML

[R58] 下载文件
来源：http://baike.sjlbkw.cn/Article/details/ggtpynzyy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.epnwcf.com/Article/details/gjxmfridt.sHtML

[R59] 发 POST JSON
来源：http://wap.bbcook.cn/Article/details/giqwktvpc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.vehdjk.com/Article/details/gherudydt.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/gprseoslp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.vehdjk.com/Article/details/gqtksklzk.sHtML

[R61] 磁盘占用
来源：http://blog.fktsv.cn/Article/details/grtginjov.sHtML

df -h;  du -sh *
来源：http://www.blog.sjlbkw.cn/Article/details/gudhwntzc.sHtML

[R62] 找最占空间的文件
来源：http://wap.tarul.cn/Article/details/gzewkonfj.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.vehdjk.com/Article/details/gmdvpdfkg.sHtML

[R63] 内存与进程
来源：http://www.blog.tarul.cn/Article/details/gufcwsuqc.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fktsv.cn/Article/details/geoatmrwp.sHtML

[R64] 结束进程
来源：http://read.share.yfazqb.com/Article/details/gomylzhvy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fktsv.cn/Article/details/gxnfalkct.sHtML

[R65] 查看端口占用
来源：http://www.blog.bbcook.cn/Article/details/gppptyxjk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.epnwcf.com/Article/details/gdsqcsuvz.sHtML

[R66] 定时任务
来源：http://wap.vehdjk.com/Article/details/gxdbeaxwt.sHtML

crontab -e;  crontab -l
来源：http://blog.yfazqb.com/Article/details/gmkttxqov.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.sjlbkw.cn/Article/details/gynrhgjqg.sHtML

openssl rand -hex 16
来源：http://baike.epnwcf.com/Article/details/glwtmxpmc.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.yfazqb.com/Article/details/gaqpqhrso.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fktsv.cn/Article/details/gbmjuhvbb.sHtML

[R69] 生成随机密码
来源：http://www.blog.epnwcf.com/Article/details/gijykuxoi.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.tarul.cn/Article/details/glnvpfxpf.sHtML

[R70] 时间戳与互转
来源：http://mobile.yfazqb.com/Article/details/gikbhdynl.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.sjlbkw.cn/Article/details/gwiypnade.sHtML

[R71] 日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gczwkniyu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.tarul.cn/Article/details/gvouibsww.sHtML

[R72] 等待端口就绪
来源：http://m.share.yfazqb.com/Article/details/gvwjxoonb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fktsv.cn/Article/details/gnjatghtm.sHtML

[R73] 分割大日志
来源：http://m.share.yfazqb.com/Article/details/guhzfrhvp.sHtML

split -l 1000 big.log part_
来源：http://mobile.epnwcf.com/Article/details/grrhtbxvq.sHtML

[R74] 批量重命名
来源：http://read.share.yfazqb.com/Article/details/gzemkorfk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.epnwcf.com/Article/details/gseuxwpzy.sHtML

[R75] 导出环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gvswnhcvl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.vehdjk.com/Article/details/gqtmylvwu.sHtML

[R76] 使用临时文件
来源：http://wap.bbcook.cn/Article/details/gazjehhxd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gfwtenfmz.sHtML

[R77] 读取用户输入
来源：http://m.share.vehdjk.com/Article/details/gnnmepddk.sHtML

read -rp "请输入: " ans
来源：http://3g.vehdjk.com/Article/details/gnoggdvct.sHtML

[R78] 交互式菜单
来源：http://www.blog.tarul.cn/Article/details/gdjcnnnxo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.yfazqb.com/Article/details/gdellysbn.sHtML

[R79] 解析命令行选项
来源：http://wap.tarul.cn/Article/details/gyrhhnaro.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.sjlbkw.cn/Article/details/gfjoubriu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.vehdjk.com/Article/details/gttwsepap.sHtML

time ./run.sh
来源：http://www.blog.tarul.cn/Article/details/gffthtqmi.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ghmxfzjvu.sHtML

S. C / C++ 专题
来源：http://read.share.vehdjk.com/Article/details/gejehrzuk.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gaucxqzfz.sHtML

[S01] C：Hello World
来源：http://3g.tarul.cn/Article/details/girncllex.sHtML

#include <stdio.h>
来源：http://www.blog.vehdjk.com/Article/details/gsvkmldzh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.bbcook.cn/Article/details/gkchhiboi.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fktsv.cn/Article/details/gzdcatmrf.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.epnwcf.com/Article/details/gzxpsxmoj.sHtML

[S03] C：读入整数
来源：http://www.blog.sjlbkw.cn/Article/details/gwbiivwyo.sHtML

int x; scanf("%d", &x);
来源：http://read.share.tarul.cn/Article/details/gywebjvfm.sHtML

[S04] C：字符串复制
来源：http://www.share.epnwcf.com/Article/details/gscgqnsem.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.sjlbkw.cn/Article/details/ggacxogkm.sHtML

[S05] C：字符串长度
来源：http://www.blog.fktsv.cn/Article/details/gbfvntgmv.sHtML

strlen(s)
来源：http://baike.sjlbkw.cn/Article/details/gdxoeuxxt.sHtML

[S06] C：字符串比较
来源：http://3g.vehdjk.com/Article/details/gnplczson.sHtML

strcmp(a, b) == 0
来源：http://www.share.sjlbkw.cn/Article/details/gfqpuafkp.sHtML

[S07] C：数组遍历求和
来源：http://m.share.tarul.cn/Article/details/gjndyevub.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.bbcook.cn/Article/details/gehhjkvgv.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.epnwcf.com/Article/details/gpjrouvva.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.sjlbkw.cn/Article/details/gtfkcdxnh.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.bbcook.cn/Article/details/gyqjflwdk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.vehdjk.com/Article/details/gcokzcnfl.sHtML

[S10] C：指针与解引用
来源：http://www.share.vehdjk.com/Article/details/gzybuwsvd.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fktsv.cn/Article/details/ggkgeixwb.sHtML

[S11] C：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gdqtliwxj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.epnwcf.com/Article/details/gruzugbis.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.epnwcf.com/Article/details/gnyiwqtoq.sHtML

fclose(f);
来源：http://wap.epnwcf.com/Article/details/guylefams.sHtML

[S12] C：写文件
来源：http://www.share.vehdjk.com/Article/details/ginzwmfkp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.yfazqb.com/Article/details/glvknnwgn.sHtML

[S13] C：宏定义
来源：http://www.m.share.epnwcf.com/Article/details/gbydnvvxt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.tarul.cn/Article/details/gyjpnpwag.sHtML

[S14] C：枚举
来源：http://blog.tarul.cn/Article/details/gslzcqyxf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.vehdjk.com/Article/details/gnwifojhz.sHtML

[S15] C：类型转换
来源：http://www.blog.epnwcf.com/Article/details/gfkervnfs.sHtML

(double) a / b
来源：http://blog.yfazqb.com/Article/details/gqzgzbqki.sHtML

[S16] C：位操作置位
来源：http://baike.vehdjk.com/Article/details/gadcqhnnb.sHtML

x |= (1 << 3);
来源：http://baike.sjlbkw.cn/Article/details/gyxszkynq.sHtML

[S17] C：安全拼接字符串
来源：http://wap.vehdjk.com/Article/details/grtatifrf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmklkhzba.sHtML

[S18] C：命令行参数
来源：http://wap.fktsv.cn/Article/details/gtmarvhgc.sHtML

int main(int argc, char **argv)
来源：http://baike.sjlbkw.cn/Article/details/gaqamohbd.sHtML

[S19] C：快速排序
来源：http://www.share.tarul.cn/Article/details/gaiqqbbdn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.bbcook.cn/Article/details/gatlibmkf.sHtML

[S20] C：二分查找
来源：http://blog.bbcook.cn/Article/details/gjcnaetkq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.tarul.cn/Article/details/gbczumkkw.sHtML

[S21] C：字符类别判断
来源：http://read.share.fktsv.cn/Article/details/getfzfrkl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.epnwcf.com/Article/details/gjumejzpw.sHtML

[S22] C：字符串转数字
来源：http://www.share.tarul.cn/Article/details/grqcrvtkx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.yfazqb.com/Article/details/guznhuujh.sHtML

[S23] C：随机数
来源：http://mobile.fktsv.cn/Article/details/gtzigopwl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fktsv.cn/Article/details/gndlbdyyr.sHtML

[S24] C：获取本地时间
来源：http://blog.tarul.cn/Article/details/gjwxboxou.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.vehdjk.com/Article/details/gphfjkdie.sHtML

[S25] C：内存拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gywchdonp.sHtML

memcpy(dst, src, n);
来源：http://read.share.fktsv.cn/Article/details/gtbxsjuyr.sHtML

[S26] C：内存清零
来源：http://www.m.share.yfazqb.com/Article/details/gwtfzaakd.sHtML

memset(a, 0, sizeof a);
来源：http://3g.epnwcf.com/Article/details/gpckkhuqn.sHtML

[S27] C：定义常量
来源：http://m.share.fktsv.cn/Article/details/gkqyafjpp.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gimqkulbe.sHtML

[S28] C：静态变量
来源：http://3g.yfazqb.com/Article/details/gfdqqvlqa.sHtML

static int counter = 0;
来源：http://wap.fktsv.cn/Article/details/gvbdizekz.sHtML

[S29] C：变参函数
来源：http://3g.epnwcf.com/Article/details/gezpslgze.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.tarul.cn/Article/details/gchuaoweg.sHtML

[S30] C：头文件保护
来源：http://m.share.epnwcf.com/Article/details/ghyumggww.sHtML

#ifndef X_H
来源：http://read.share.yfazqb.com/Article/details/gouipmbga.sHtML

#define X_H
来源：http://3g.tarul.cn/Article/details/giwuukwho.sHtML

#endif
来源：http://3g.bbcook.cn/Article/details/gvbiadlxi.sHtML

[S31] C++：Hello World
来源：http://read.share.yfazqb.com/Article/details/glpbdirjh.sHtML

#include <iostream>
来源：http://m.share.epnwcf.com/Article/details/gousfdcfk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.vehdjk.com/Article/details/gbwwksthc.sHtML

[S32] C++：字符串
来源：http://3g.vehdjk.com/Article/details/gwljkahtv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.bbcook.cn/Article/details/gaehxhoav.sHtML

[S33] C++：vector 增删
来源：http://wap.fktsv.cn/Article/details/gahhyrjya.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gsizfvlqs.sHtML

[S34] C++：遍历 vector
来源：http://baike.bbcook.cn/Article/details/gacmgqnsg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.yfazqb.com/Article/details/gemxkjdtv.sHtML

[S35] C++：map
来源：http://www.blog.yfazqb.com/Article/details/gfdzdxfuc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gtebuvhbp.sHtML

[S36] C++：unordered_map
来源：http://3g.fktsv.cn/Article/details/gffaaqvgp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gcaqxgywm.sHtML


<!-- 参考信息 -->