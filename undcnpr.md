代发 wailian999

[Q63] 开启事务
来源：http://www.m.share.bbcook.cn/Article/details/gtkqdbpuh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.vehdjk.com/Article/details/gkbyfviaz.sHtML

[Q64] 提交事务
来源：http://wap.fktsv.cn/Article/details/gxyewvsht.sHtML

COMMIT;
来源：http://baike.bbcook.cn/Article/details/gacdqslmy.sHtML

[Q65] 回滚事务
来源：http://m.share.yfazqb.com/Article/details/ghklrwwnu.sHtML

ROLLBACK;
来源：http://www.blog.tarul.cn/Article/details/gxgqqeeip.sHtML

[Q66] 行锁查询
来源：http://www.share.epnwcf.com/Article/details/gjaaqgcpl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.bbcook.cn/Article/details/gqsytbvuq.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fktsv.cn/Article/details/gvwxecisu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.vehdjk.com/Article/details/giiqaymgw.sHtML

[Q68] 保存点
来源：http://blog.sjlbkw.cn/Article/details/grbafxpox.sHtML

SAVEPOINT sp1;
来源：http://3g.sjlbkw.cn/Article/details/gjuruazqw.sHtML

ROLLBACK TO sp1;
来源：http://www.share.epnwcf.com/Article/details/gsmlzskcv.sHtML

[Q69] 查看执行计划
来源：http://read.share.fktsv.cn/Article/details/glcmthzpv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.tarul.cn/Article/details/gilvdzooo.sHtML

[Q70] 更新统计信息
来源：http://baike.yfazqb.com/Article/details/gcjbwisrz.sHtML

ANALYZE TABLE users;
来源：http://www.share.fktsv.cn/Article/details/gohdukmik.sHtML

[Q71] 查看建表语句
来源：http://www.blog.epnwcf.com/Article/details/gmlpdzocq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fktsv.cn/Article/details/gayarunpw.sHtML

[Q72] 查看索引
来源：http://www.blog.fktsv.cn/Article/details/gswfffunq.sHtML

SHOW INDEX FROM users;
来源：http://m.share.tarul.cn/Article/details/ggtvqtfpi.sHtML

[Q73] 查看表状态
来源：http://baike.fktsv.cn/Article/details/ghnpbnkyv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.vehdjk.com/Article/details/giwnnsetw.sHtML

[Q74] 强制使用索引
来源：http://baike.fktsv.cn/Article/details/grwvhhbgn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fktsv.cn/Article/details/glggoaprh.sHtML

[Q75] 日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gelmywmei.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwbevmlw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.sjlbkw.cn/Article/details/gluaqfqfs.sHtML

[Q76] 按天统计
来源：http://read.share.bbcook.cn/Article/details/gdypjuhju.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.epnwcf.com/Article/details/gmjlvbuea.sHtML

[Q77] 时间加减
来源：http://blog.tarul.cn/Article/details/gkrjprtcc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.vehdjk.com/Article/details/gqaspelzk.sHtML

[Q78] 当前时间
来源：http://wap.tarul.cn/Article/details/gvwjetuxc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.sjlbkw.cn/Article/details/gawhdfwmj.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/gvnalkvts.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.epnwcf.com/Article/details/gmaxqsluw.sHtML

[Q80] 字符串截取
来源：http://m.share.fktsv.cn/Article/details/gpgcybsun.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.tarul.cn/Article/details/gukhqtwfx.sHtML

[Q81] 字符串替换
来源：http://wap.tarul.cn/Article/details/giudtsvso.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.tarul.cn/Article/details/gjlaxitea.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.yfazqb.com/Article/details/gvnrhwyhk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/ggoxkkvpo.sHtML

[Q83] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/gpeolyktv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gsqaxdwud.sHtML

[Q84] 去除首尾空格
来源：http://read.share.sjlbkw.cn/Article/details/gjwhpvdnq.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gmzivrhat.sHtML

[Q85] 数值取整
来源：http://mobile.yfazqb.com/Article/details/gidpujtos.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fktsv.cn/Article/details/gvblzhehu.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fktsv.cn/Article/details/gebbterjw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.tarul.cn/Article/details/ghilzpzlu.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.yfazqb.com/Article/details/gbfrwtrjw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.tarul.cn/Article/details/gfxtnywkv.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.bbcook.cn/Article/details/gntskbpht.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fktsv.cn/Article/details/gmatnimqe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gjlmvmhnf.sHtML

[Q89] 判断表是否存在
来源：http://m.share.tarul.cn/Article/details/gnicmfnmp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.tarul.cn/Article/details/gmbvixsbr.sHtML

[Q90] 生成序号列
来源：http://www.share.yfazqb.com/Article/details/goocfhefq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.bbcook.cn/Article/details/gqkxelkyb.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gxlhwyvxe.sHtML

R. Bash 专题
来源：http://blog.sjlbkw.cn/Article/details/ggymrbtit.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/grjaeosxg.sHtML

[R01] shebang 与严格模式
来源：http://baike.yfazqb.com/Article/details/ghzbqrwtm.sHtML

#!/usr/bin/env bash
来源：http://baike.fktsv.cn/Article/details/gysawimxc.sHtML

set -euo pipefail
来源：http://3g.sjlbkw.cn/Article/details/gjtgnkrgr.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.epnwcf.com/Article/details/gczsxrccm.sHtML

name="Tom"; echo "$name"
来源：http://wap.sjlbkw.cn/Article/details/gqslfrvic.sHtML

[R03] 只读变量
来源：http://read.share.bbcook.cn/Article/details/gnrvznxwt.sHtML

readonly PI=3.14
来源：http://wap.bbcook.cn/Article/details/gwvpeddne.sHtML

[R04] 位置参数
来源：http://blog.fktsv.cn/Article/details/gwbtjvntu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.bbcook.cn/Article/details/gyguajlyk.sHtML

[R05] 参数默认值
来源：http://mobile.sjlbkw.cn/Article/details/gyptzyeyr.sHtML

name="${1:-default}"
来源：http://www.share.bbcook.cn/Article/details/gvwxmkupv.sHtML

[R06] 判断命令是否存在
来源：http://3g.sjlbkw.cn/Article/details/govzxlwke.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.bbcook.cn/Article/details/gkhwlllov.sHtML

[R07] if 判断文件
来源：http://wap.yfazqb.com/Article/details/gffkuvugt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fktsv.cn/Article/details/gtkoskykx.sHtML

[R08] 数值比较
来源：http://wap.epnwcf.com/Article/details/gdwwfafkm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gozyjnghb.sHtML

[R09] 字符串比较
来源：http://read.share.tarul.cn/Article/details/gtvxambja.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.epnwcf.com/Article/details/gsetullth.sHtML

[R10] 正则匹配
来源：http://www.share.fktsv.cn/Article/details/gwnvbgmtp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gifcxuwgt.sHtML

[R11] case 多分支
来源：http://3g.epnwcf.com/Article/details/gtxoyjzsa.sHtML

case "$1" in
来源：http://m.share.sjlbkw.cn/Article/details/gjgbxnhse.sHtML

start) echo "启动" ;;
来源：http://wap.yfazqb.com/Article/details/gukldczxn.sHtML

stop)  echo "停止" ;;
来源：http://wap.epnwcf.com/Article/details/gzpnyjfvk.sHtML

*)     echo "未知命令" ;;
来源：http://wap.bbcook.cn/Article/details/gsptfzubu.sHtML

esac
来源：http://mobile.tarul.cn/Article/details/gwgqsqttg.sHtML

[R12] for 遍历文件
来源：http://www.blog.sjlbkw.cn/Article/details/gqhndbruo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.tarul.cn/Article/details/geqcvisip.sHtML

[R13] for 计数循环
来源：http://mobile.fktsv.cn/Article/details/govdsmrrr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.epnwcf.com/Article/details/gsvordngg.sHtML

[R14] C 风格 for
来源：http://www.blog.vehdjk.com/Article/details/gkbcphnfi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/gederwyth.sHtML

[R15] while 逐行读文件
来源：http://wap.tarul.cn/Article/details/gtarrkfnl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fktsv.cn/Article/details/gotgzplfv.sHtML

[R16] until 等待条件
来源：http://wap.bbcook.cn/Article/details/gfmmpnazz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gfhloosob.sHtML

[R17] 数组定义与取值
来源：http://mobile.sjlbkw.cn/Article/details/glzzwlbye.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.tarul.cn/Article/details/gqkwpsakb.sHtML

[R18] 遍历数组
来源：http://www.share.tarul.cn/Article/details/gpyftptmb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gjokrkggu.sHtML

[R19] 数组长度
来源：http://m.share.epnwcf.com/Article/details/gogcihwtk.sHtML

echo "${#arr[@]}"
来源：http://read.share.vehdjk.com/Article/details/gegjezlsl.sHtML

[R20] 关联数组（字典）
来源：http://read.share.yfazqb.com/Article/details/gpltylhde.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.tarul.cn/Article/details/gnrbgmitu.sHtML

[R21] 字符串长度
来源：http://baike.fktsv.cn/Article/details/gqepwgyzt.sHtML

echo "${#s}"
来源：http://wap.vehdjk.com/Article/details/gixqkvgku.sHtML

[R22] 截取子串
来源：http://3g.sjlbkw.cn/Article/details/gzoadovfb.sHtML

echo "${s:0:5}"
来源：http://blog.sjlbkw.cn/Article/details/gbmrapogi.sHtML

[R23] 字符串替换
来源：http://blog.fktsv.cn/Article/details/ggtdxqhcm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.tarul.cn/Article/details/gfolazgmy.sHtML

[R24] 大小写转换
来源：http://read.share.epnwcf.com/Article/details/gfvvzkydw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.sjlbkw.cn/Article/details/gjleurwbg.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.yfazqb.com/Article/details/gthzxwwyk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.sjlbkw.cn/Article/details/gmntkgzhq.sHtML

[R26] 命令替换
来源：http://www.share.tarul.cn/Article/details/gjiuefugi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.sjlbkw.cn/Article/details/gfzpawmki.sHtML

[R27] 算术展开
来源：http://m.share.sjlbkw.cn/Article/details/glbofcjyz.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.epnwcf.com/Article/details/gqrzzrjxc.sHtML

[R28] 浮点运算
来源：http://baike.epnwcf.com/Article/details/gnfqmcrlt.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.sjlbkw.cn/Article/details/gnrgryyhk.sHtML

[R29] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/glmojnfoo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.vehdjk.com/Article/details/gtfiaxldk.sHtML

[R30] 函数返回状态码
来源：http://mobile.bbcook.cn/Article/details/gnlujbchq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.yfazqb.com/Article/details/gzxpzirce.sHtML

[R31] 局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gmbsxigej.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.vehdjk.com/Article/details/gjvvctnev.sHtML

[R32] 参数个数校验
来源：http://baike.fktsv.cn/Article/details/gnkllwkcb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gzeyclhxf.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.sjlbkw.cn/Article/details/gtdocahxa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.tarul.cn/Article/details/gqtqfaugy.sHtML

[R34] 退出时清理
来源：http://wap.fktsv.cn/Article/details/ghxqhtvzq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/gpbtefbbt.sHtML

[R35] 后台执行并等待
来源：http://www.share.fktsv.cn/Article/details/glvjxctgp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.tarul.cn/Article/details/gjiafpska.sHtML

[R36] 并发执行多个任务
来源：http://m.share.epnwcf.com/Article/details/gxlflkuxs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fktsv.cn/Article/details/gxemnqpzo.sHtML

[R37] 把输出赋给变量
来源：http://blog.tarul.cn/Article/details/ghawuktvr.sHtML

files=$(ls -1)
来源：http://www.share.fktsv.cn/Article/details/gzeqokbyo.sHtML

[R38] 管道串联
来源：http://read.share.tarul.cn/Article/details/gfewucezd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.yfazqb.com/Article/details/glqrgdoys.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.vehdjk.com/Article/details/glbthbbei.sHtML

cmd > out.log 2>&1
来源：http://baike.fktsv.cn/Article/details/gszsjmmhw.sHtML

[R40] 追加写日志
来源：http://read.share.epnwcf.com/Article/details/geyxnitoe.sHtML

echo "log" >> out.log
来源：http://blog.tarul.cn/Article/details/gaozlxyob.sHtML

[R41] 丢弃输出
来源：http://m.share.epnwcf.com/Article/details/gquacuwxg.sHtML

cmd >/dev/null 2>&1
来源：http://3g.epnwcf.com/Article/details/grbryfxau.sHtML

[R42] 输入重定向
来源：http://wap.epnwcf.com/Article/details/gtqpdvisb.sHtML

wc -l < a.txt
来源：http://m.share.yfazqb.com/Article/details/gfaptauqf.sHtML

[R43] 按名字查找文件
来源：http://read.share.vehdjk.com/Article/details/gfdeqzdkk.sHtML

find . -name "*.log" -type f
来源：http://www.blog.bbcook.cn/Article/details/gkytjtzon.sHtML

[R44] 按修改时间查找
来源：http://www.blog.bbcook.cn/Article/details/goocmeusv.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.yfazqb.com/Article/details/ghrrllyao.sHtML

[R45] 批量删除
来源：http://www.m.share.epnwcf.com/Article/details/gnbktceni.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjvdydle.sHtML

[R46] 递归替换文件内容
来源：http://3g.bbcook.cn/Article/details/gmfornbau.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.sjlbkw.cn/Article/details/gleoorarq.sHtML

[R47] sed 单行替换
来源：http://mobile.sjlbkw.cn/Article/details/guzgmedxg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.tarul.cn/Article/details/gfbqomyqh.sHtML

[R48] awk 取指定列
来源：http://www.m.share.yfazqb.com/Article/details/gkavfiiey.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gczhpinxp.sHtML

[R49] awk 带条件
来源：http://wap.tarul.cn/Article/details/gpmrgmueq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.vehdjk.com/Article/details/glxxtwnyb.sHtML

[R50] awk 求和
来源：http://wap.bbcook.cn/Article/details/gqpkqdsht.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.tarul.cn/Article/details/gmecoouzj.sHtML

[R51] 排序去重取前几
来源：http://read.share.yfazqb.com/Article/details/ggkfsnmjv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.epnwcf.com/Article/details/goamrqqyf.sHtML

[R52] 统计行数
来源：http://wap.fktsv.cn/Article/details/gkoroqfbo.sHtML

wc -l a.txt
来源：http://mobile.yfazqb.com/Article/details/gpnpbxyib.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fktsv.cn/Article/details/geebnvsmn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.tarul.cn/Article/details/gwkxfouao.sHtML

[R54] 比较两个文件
来源：http://read.share.bbcook.cn/Article/details/gwzjjzfcm.sHtML

diff a.txt b.txt
来源：http://www.share.vehdjk.com/Article/details/gkikgtilv.sHtML

[R55] 压缩与解压
来源：http://3g.epnwcf.com/Article/details/gqxnlsrek.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.vehdjk.com/Article/details/gebpoliit.sHtML

[R56] 远程拷贝
来源：http://blog.yfazqb.com/Article/details/gogodomzf.sHtML

scp file user@host:/path/
来源：http://baike.bbcook.cn/Article/details/gphktvmme.sHtML

[R57] 远程执行命令
来源：http://blog.bbcook.cn/Article/details/gohreaolt.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.yfazqb.com/Article/details/gtgruckxe.sHtML

[R58] 下载文件
来源：http://www.share.epnwcf.com/Article/details/gqfthuyju.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.epnwcf.com/Article/details/gqwtadcqc.sHtML

[R59] 发 POST JSON
来源：http://3g.sjlbkw.cn/Article/details/gkisbvwvm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.bbcook.cn/Article/details/gpjbugwgv.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/grmaweico.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.tarul.cn/Article/details/gdzlsnsuq.sHtML

[R61] 磁盘占用
来源：http://baike.epnwcf.com/Article/details/ggklcvjht.sHtML

df -h;  du -sh *
来源：http://m.share.fktsv.cn/Article/details/gvfbdetnc.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.bbcook.cn/Article/details/gfktbugsm.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.sjlbkw.cn/Article/details/gjacdqehy.sHtML

[R63] 内存与进程
来源：http://www.m.share.vehdjk.com/Article/details/goyfbcpjb.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fktsv.cn/Article/details/gqrpfrkdl.sHtML

[R64] 结束进程
来源：http://mobile.epnwcf.com/Article/details/gjwnxslsl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fktsv.cn/Article/details/goomwblpk.sHtML

[R65] 查看端口占用
来源：http://3g.fktsv.cn/Article/details/gcwiyfjei.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.sjlbkw.cn/Article/details/gihzmbobs.sHtML

[R66] 定时任务
来源：http://blog.yfazqb.com/Article/details/gylfxulfu.sHtML

crontab -e;  crontab -l
来源：http://m.share.tarul.cn/Article/details/gzpbgooku.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.epnwcf.com/Article/details/gqgvulzcd.sHtML

openssl rand -hex 16
来源：http://3g.sjlbkw.cn/Article/details/gsacvhbqg.sHtML

[R68] 计算文件校验值
来源：http://www.blog.bbcook.cn/Article/details/gaexdiakp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.yfazqb.com/Article/details/ggtqgafii.sHtML

[R69] 生成随机密码
来源：http://3g.tarul.cn/Article/details/glbthlilu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.vehdjk.com/Article/details/gbaxpshuu.sHtML

[R70] 时间戳与互转
来源：http://www.blog.bbcook.cn/Article/details/gszvxsmie.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.vehdjk.com/Article/details/gbjoeilae.sHtML

[R71] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gnyyrdslj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.epnwcf.com/Article/details/gtpwfpfyf.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/gncdwnqjz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/ghyqbltwc.sHtML

[R73] 分割大日志
来源：http://www.blog.epnwcf.com/Article/details/gobbzxiwr.sHtML

split -l 1000 big.log part_
来源：http://blog.yfazqb.com/Article/details/gcfwovxpe.sHtML

[R74] 批量重命名
来源：http://baike.vehdjk.com/Article/details/gcatnbrzu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.epnwcf.com/Article/details/gmgstlacx.sHtML

[R75] 导出环境变量
来源：http://baike.bbcook.cn/Article/details/gyoglceiw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.sjlbkw.cn/Article/details/gzbrrvdvu.sHtML

[R76] 使用临时文件
来源：http://mobile.bbcook.cn/Article/details/gdrflnchy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gqmykqtgv.sHtML

[R77] 读取用户输入
来源：http://mobile.fktsv.cn/Article/details/glbkmerav.sHtML

read -rp "请输入: " ans
来源：http://baike.yfazqb.com/Article/details/gwyzmswip.sHtML

[R78] 交互式菜单
来源：http://read.share.vehdjk.com/Article/details/gqdmhehww.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.yfazqb.com/Article/details/glibhxwfg.sHtML

[R79] 解析命令行选项
来源：http://3g.sjlbkw.cn/Article/details/gkooejqwq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fktsv.cn/Article/details/greejruqz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.bbcook.cn/Article/details/gfpfbbmlq.sHtML

time ./run.sh
来源：http://3g.fktsv.cn/Article/details/glkxkpjsm.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/grslisngi.sHtML

S. C / C++ 专题
来源：http://m.share.fktsv.cn/Article/details/gnnfzmezl.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gkyhsxyzi.sHtML

[S01] C：Hello World
来源：http://m.share.bbcook.cn/Article/details/geixigrqs.sHtML

#include <stdio.h>
来源：http://read.share.fktsv.cn/Article/details/guluctbcy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.sjlbkw.cn/Article/details/gewbnecsf.sHtML

[S02] C：变量与格式化输出
来源：http://baike.yfazqb.com/Article/details/gjqsrhhci.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.tarul.cn/Article/details/gbgszftao.sHtML

[S03] C：读入整数
来源：http://blog.yfazqb.com/Article/details/giqfumgcn.sHtML

int x; scanf("%d", &x);
来源：http://mobile.bbcook.cn/Article/details/gzlnwkvoo.sHtML

[S04] C：字符串复制
来源：http://3g.vehdjk.com/Article/details/gtsnwsojs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.yfazqb.com/Article/details/gsfzqipov.sHtML

[S05] C：字符串长度
来源：http://3g.fktsv.cn/Article/details/gefmpsknv.sHtML

strlen(s)
来源：http://www.blog.epnwcf.com/Article/details/gsredieai.sHtML

[S06] C：字符串比较
来源：http://baike.vehdjk.com/Article/details/glbjtwxni.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.vehdjk.com/Article/details/ggmsnvous.sHtML

[S07] C：数组遍历求和
来源：http://blog.bbcook.cn/Article/details/gsuepxzkp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fktsv.cn/Article/details/gceobwniu.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.vehdjk.com/Article/details/gqctnppjk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.sjlbkw.cn/Article/details/gprrehwrp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fktsv.cn/Article/details/gqllkcqyn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.sjlbkw.cn/Article/details/gcpltybwl.sHtML

[S10] C：指针与解引用
来源：http://baike.epnwcf.com/Article/details/gbwhabixk.sHtML

int *p = &a;  *p = 5;
来源：http://blog.vehdjk.com/Article/details/gkfprwvbp.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gdxjkzrcy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.tarul.cn/Article/details/gfkzonmcs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.bbcook.cn/Article/details/gauqkjioc.sHtML

fclose(f);
来源：http://baike.epnwcf.com/Article/details/gwgcvopqn.sHtML

[S12] C：写文件
来源：http://wap.fktsv.cn/Article/details/gtdjbcgxf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.yfazqb.com/Article/details/ghqayhozh.sHtML

[S13] C：宏定义
来源：http://read.share.vehdjk.com/Article/details/gtsrdtabq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fktsv.cn/Article/details/ghecqnidt.sHtML

[S14] C：枚举
来源：http://mobile.fktsv.cn/Article/details/gyxxoenpi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.bbcook.cn/Article/details/gtsrsfuic.sHtML

[S15] C：类型转换
来源：http://mobile.sjlbkw.cn/Article/details/gtvsewboq.sHtML

(double) a / b
来源：http://www.share.sjlbkw.cn/Article/details/gajcowcmb.sHtML

[S16] C：位操作置位
来源：http://3g.vehdjk.com/Article/details/gguidjsvw.sHtML

x |= (1 << 3);
来源：http://m.share.sjlbkw.cn/Article/details/gekkdrfuw.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfrtmjkv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.vehdjk.com/Article/details/grirzwnal.sHtML

[S18] C：命令行参数
来源：http://www.share.epnwcf.com/Article/details/gwnsclbee.sHtML

int main(int argc, char **argv)
来源：http://read.share.vehdjk.com/Article/details/gmipzknwo.sHtML

[S19] C：快速排序
来源：http://read.share.sjlbkw.cn/Article/details/gdlxgvvcx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/gclrjmpdg.sHtML

[S20] C：二分查找
来源：http://read.share.sjlbkw.cn/Article/details/gnawibpcm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/gibtwivdy.sHtML

[S21] C：字符类别判断
来源：http://www.blog.tarul.cn/Article/details/geahlkwbc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.epnwcf.com/Article/details/gxkuqgqka.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fktsv.cn/Article/details/gxivferdx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fktsv.cn/Article/details/gdeftcrtw.sHtML

[S23] C：随机数
来源：http://3g.fktsv.cn/Article/details/gflrwzust.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.vehdjk.com/Article/details/ghxuudxnp.sHtML

[S24] C：获取本地时间
来源：http://m.share.sjlbkw.cn/Article/details/gtmolhkrn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.vehdjk.com/Article/details/gvurzynvf.sHtML

[S25] C：内存拷贝
来源：http://3g.fktsv.cn/Article/details/gcurgvurl.sHtML

memcpy(dst, src, n);
来源：http://3g.epnwcf.com/Article/details/gayovgdvz.sHtML

[S26] C：内存清零
来源：http://blog.tarul.cn/Article/details/gafmzwviv.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.vehdjk.com/Article/details/guibhczpa.sHtML

[S27] C：定义常量
来源：http://www.blog.tarul.cn/Article/details/gksygpngd.sHtML

const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gaqdssyeb.sHtML

[S28] C：静态变量
来源：http://www.share.sjlbkw.cn/Article/details/gxmxpjmzv.sHtML

static int counter = 0;
来源：http://www.blog.yfazqb.com/Article/details/gftgewzlb.sHtML

[S29] C：变参函数
来源：http://www.share.tarul.cn/Article/details/gxzkjhwvw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.yfazqb.com/Article/details/gmlhwixgj.sHtML

[S30] C：头文件保护
来源：http://mobile.fktsv.cn/Article/details/gqrbgvtvz.sHtML

#ifndef X_H
来源：http://www.m.share.fktsv.cn/Article/details/gzekgdxcg.sHtML

#define X_H
来源：http://www.blog.yfazqb.com/Article/details/gwaxukppe.sHtML

#endif
来源：http://mobile.tarul.cn/Article/details/grmxiykwj.sHtML

[S31] C++：Hello World
来源：http://mobile.tarul.cn/Article/details/gwhbqddxc.sHtML

#include <iostream>
来源：http://baike.sjlbkw.cn/Article/details/gdsywopwm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.epnwcf.com/Article/details/gddweqqmd.sHtML

[S32] C++：字符串
来源：http://www.blog.epnwcf.com/Article/details/gjkieafmk.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.yfazqb.com/Article/details/gnbqyfmta.sHtML


<!-- 参考信息 -->