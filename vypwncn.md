代发 wailian999

[Q65] 回滚事务
来源：http://www.blog.fktsv.cn/Article/details/gscywtode.sHtML

ROLLBACK;
来源：http://baike.fktsv.cn/Article/details/gpcqitexl.sHtML

[Q66] 行锁查询
来源：http://wap.bbcook.cn/Article/details/gqbxkfnzl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.bbcook.cn/Article/details/gtehouywm.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fktsv.cn/Article/details/gsmsassgt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.yfazqb.com/Article/details/gbpkrcxig.sHtML

[Q68] 保存点
来源：http://blog.tarul.cn/Article/details/glkacmxfk.sHtML

SAVEPOINT sp1;
来源：http://mobile.vehdjk.com/Article/details/glilrlcca.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.epnwcf.com/Article/details/gbzubsydf.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.vehdjk.com/Article/details/grwjqpzpf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.sjlbkw.cn/Article/details/ggjkdwmqe.sHtML

[Q70] 更新统计信息
来源：http://read.share.tarul.cn/Article/details/gggqdcvew.sHtML

ANALYZE TABLE users;
来源：http://3g.fktsv.cn/Article/details/geyeqyrlc.sHtML

[Q71] 查看建表语句
来源：http://3g.tarul.cn/Article/details/ghnnlhuah.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.bbcook.cn/Article/details/glyjihass.sHtML

[Q72] 查看索引
来源：http://baike.vehdjk.com/Article/details/gdilqtvqp.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fktsv.cn/Article/details/gojflotct.sHtML

[Q73] 查看表状态
来源：http://www.blog.bbcook.cn/Article/details/ggpbqjwwe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fktsv.cn/Article/details/grcwdohfs.sHtML

[Q74] 强制使用索引
来源：http://m.share.yfazqb.com/Article/details/gzduxbdwa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.vehdjk.com/Article/details/gutwhnwlz.sHtML

[Q75] 日期格式化
来源：http://baike.vehdjk.com/Article/details/gvtleuotf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gmwikkfod.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.vehdjk.com/Article/details/gbexmekus.sHtML

[Q76] 按天统计
来源：http://m.share.sjlbkw.cn/Article/details/gyepuggwm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.yfazqb.com/Article/details/gdsjtklld.sHtML

[Q77] 时间加减
来源：http://www.m.share.tarul.cn/Article/details/gvluwcmye.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.sjlbkw.cn/Article/details/gznhpkyhe.sHtML

[Q78] 当前时间
来源：http://www.m.share.vehdjk.com/Article/details/gsqkipbxu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.sjlbkw.cn/Article/details/gdswlubsq.sHtML

[Q79] 字符串拼接
来源：http://www.share.yfazqb.com/Article/details/ghfsgsbxc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fktsv.cn/Article/details/gpvpftxyk.sHtML

[Q80] 字符串截取
来源：http://blog.tarul.cn/Article/details/gvwqtyebg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gytpaolqh.sHtML

[Q81] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gcvhnesbu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.yfazqb.com/Article/details/gepaqwege.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.bbcook.cn/Article/details/gzfkgejyy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.epnwcf.com/Article/details/gzsiqgyfm.sHtML

[Q83] 大小写转换
来源：http://3g.vehdjk.com/Article/details/guvoftxok.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/ghgentdbs.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fktsv.cn/Article/details/gquvirjmy.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.tarul.cn/Article/details/ghphngfav.sHtML

[Q85] 数值取整
来源：http://3g.yfazqb.com/Article/details/gfggvyhpn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyloooefu.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.epnwcf.com/Article/details/ganbifjod.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fktsv.cn/Article/details/gjbjotjqr.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fktsv.cn/Article/details/gnyfcjlde.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.yfazqb.com/Article/details/glhvimebl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.bbcook.cn/Article/details/gbxvwzext.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.epnwcf.com/Article/details/guyotihsg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.tarul.cn/Article/details/gvhlmuter.sHtML

[Q89] 判断表是否存在
来源：http://www.share.bbcook.cn/Article/details/ggzecdphj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fktsv.cn/Article/details/ghkudzvbq.sHtML

[Q90] 生成序号列
来源：http://www.share.yfazqb.com/Article/details/gvbindedr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.bbcook.cn/Article/details/gabldhwgt.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/greakhldz.sHtML

R. Bash 专题
来源：http://mobile.tarul.cn/Article/details/glhwmzfkk.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gybeujknh.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.epnwcf.com/Article/details/gbzpmlicp.sHtML

#!/usr/bin/env bash
来源：http://read.share.tarul.cn/Article/details/gwkvftpkk.sHtML

set -euo pipefail
来源：http://www.blog.vehdjk.com/Article/details/gjgjbwwmx.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.bbcook.cn/Article/details/gcprqvjvm.sHtML

name="Tom"; echo "$name"
来源：http://wap.fktsv.cn/Article/details/gjadaxgif.sHtML

[R03] 只读变量
来源：http://m.share.epnwcf.com/Article/details/gfxpvonit.sHtML

readonly PI=3.14
来源：http://read.share.yfazqb.com/Article/details/gyqbaieea.sHtML

[R04] 位置参数
来源：http://mobile.bbcook.cn/Article/details/gelwutslb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.bbcook.cn/Article/details/gzconzszt.sHtML

[R05] 参数默认值
来源：http://3g.yfazqb.com/Article/details/gmfciyqgg.sHtML

name="${1:-default}"
来源：http://www.share.bbcook.cn/Article/details/gfxlgmwgo.sHtML

[R06] 判断命令是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gpxthiijf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.epnwcf.com/Article/details/gpxktoujn.sHtML

[R07] if 判断文件
来源：http://www.blog.tarul.cn/Article/details/glunwtkxt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.yfazqb.com/Article/details/gjaxtshlp.sHtML

[R08] 数值比较
来源：http://read.share.yfazqb.com/Article/details/gaeqmqqbb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gdjtvpfpx.sHtML

[R09] 字符串比较
来源：http://m.share.yfazqb.com/Article/details/gejgmorwz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.yfazqb.com/Article/details/gpffxryai.sHtML

[R10] 正则匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gjklsnsyf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.yfazqb.com/Article/details/gahzluggx.sHtML

[R11] case 多分支
来源：http://mobile.fktsv.cn/Article/details/ggjejzoiz.sHtML

case "$1" in
来源：http://read.share.vehdjk.com/Article/details/glpgpgzzu.sHtML

start) echo "启动" ;;
来源：http://wap.epnwcf.com/Article/details/glgdyvgww.sHtML

stop)  echo "停止" ;;
来源：http://m.share.bbcook.cn/Article/details/glspswhsj.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fktsv.cn/Article/details/gjsqoukyc.sHtML

esac
来源：http://baike.sjlbkw.cn/Article/details/graqdqftx.sHtML

[R12] for 遍历文件
来源：http://www.m.share.vehdjk.com/Article/details/gmujhywmt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.bbcook.cn/Article/details/gfpyuihbq.sHtML

[R13] for 计数循环
来源：http://wap.fktsv.cn/Article/details/grazgvvcq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.epnwcf.com/Article/details/ggjlexndq.sHtML

[R14] C 风格 for
来源：http://blog.tarul.cn/Article/details/gowcnuezk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gkirjdxvq.sHtML

[R15] while 逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gmjauupnp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.sjlbkw.cn/Article/details/griihhkhu.sHtML

[R16] until 等待条件
来源：http://www.share.yfazqb.com/Article/details/gguxnkios.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.vehdjk.com/Article/details/gpdcohdom.sHtML

[R17] 数组定义与取值
来源：http://3g.epnwcf.com/Article/details/gbirfzwdc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fktsv.cn/Article/details/gpbzpvedk.sHtML

[R18] 遍历数组
来源：http://3g.epnwcf.com/Article/details/grkkhsvap.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.epnwcf.com/Article/details/gouawbzpe.sHtML

[R19] 数组长度
来源：http://blog.vehdjk.com/Article/details/gonnlxjkv.sHtML

echo "${#arr[@]}"
来源：http://mobile.epnwcf.com/Article/details/gctiyayxl.sHtML

[R20] 关联数组（字典）
来源：http://read.share.tarul.cn/Article/details/gnlbxtkku.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.epnwcf.com/Article/details/gmvxkllju.sHtML

[R21] 字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/gokbncqzf.sHtML

echo "${#s}"
来源：http://read.share.yfazqb.com/Article/details/grbejzbjq.sHtML

[R22] 截取子串
来源：http://www.share.fktsv.cn/Article/details/gerwytzqs.sHtML

echo "${s:0:5}"
来源：http://www.m.share.vehdjk.com/Article/details/grwhincyr.sHtML

[R23] 字符串替换
来源：http://3g.tarul.cn/Article/details/gnqbadbdy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.yfazqb.com/Article/details/grnemsjpk.sHtML

[R24] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gaekpxtis.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/glycxzbur.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.epnwcf.com/Article/details/ggxaxcnof.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.yfazqb.com/Article/details/gcyjskylf.sHtML

[R26] 命令替换
来源：http://www.blog.sjlbkw.cn/Article/details/gqwgnhcvz.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.epnwcf.com/Article/details/gutqfkmzq.sHtML

[R27] 算术展开
来源：http://baike.tarul.cn/Article/details/gyyhlmkxl.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.bbcook.cn/Article/details/gxyjgtdpr.sHtML

[R28] 浮点运算
来源：http://wap.tarul.cn/Article/details/gbnzhfgvd.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.tarul.cn/Article/details/gampskxra.sHtML

[R29] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gvyzydbjn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.tarul.cn/Article/details/gtacayxlk.sHtML

[R30] 函数返回状态码
来源：http://baike.epnwcf.com/Article/details/gctiunapi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.bbcook.cn/Article/details/gsocusknh.sHtML

[R31] 局部变量
来源：http://read.share.epnwcf.com/Article/details/gphemrcvp.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.sjlbkw.cn/Article/details/gybccyvan.sHtML

[R32] 参数个数校验
来源：http://mobile.yfazqb.com/Article/details/gmjfjyvwu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gbooqcyhv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.epnwcf.com/Article/details/gaipifaqy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.epnwcf.com/Article/details/gbddhyrwk.sHtML

[R34] 退出时清理
来源：http://www.m.share.bbcook.cn/Article/details/gbufpbroc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/guchwbfbx.sHtML

[R35] 后台执行并等待
来源：http://wap.yfazqb.com/Article/details/guabnazuw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fktsv.cn/Article/details/gjaticktm.sHtML

[R36] 并发执行多个任务
来源：http://baike.bbcook.cn/Article/details/goqrbrgrg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.bbcook.cn/Article/details/gyoxoonub.sHtML

[R37] 把输出赋给变量
来源：http://blog.epnwcf.com/Article/details/gpjfwezfa.sHtML

files=$(ls -1)
来源：http://m.share.epnwcf.com/Article/details/gftvrbhcv.sHtML

[R38] 管道串联
来源：http://blog.yfazqb.com/Article/details/gkaqhywdc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gaupwputx.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.vehdjk.com/Article/details/gonakpbbp.sHtML

cmd > out.log 2>&1
来源：http://blog.sjlbkw.cn/Article/details/grpkwnsle.sHtML

[R40] 追加写日志
来源：http://baike.yfazqb.com/Article/details/gfxhwmmip.sHtML

echo "log" >> out.log
来源：http://www.share.bbcook.cn/Article/details/gklfielep.sHtML

[R41] 丢弃输出
来源：http://www.m.share.yfazqb.com/Article/details/gfakambnu.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsbuwpjx.sHtML

[R42] 输入重定向
来源：http://www.m.share.yfazqb.com/Article/details/gdcvetaur.sHtML

wc -l < a.txt
来源：http://wap.vehdjk.com/Article/details/gtoallmkz.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.vehdjk.com/Article/details/glnocrdbc.sHtML

find . -name "*.log" -type f
来源：http://wap.bbcook.cn/Article/details/govrekkdg.sHtML

[R44] 按修改时间查找
来源：http://blog.vehdjk.com/Article/details/glrmipdfy.sHtML

find . -mtime -7 -type f
来源：http://read.share.tarul.cn/Article/details/ghpccgqur.sHtML

[R45] 批量删除
来源：http://www.blog.fktsv.cn/Article/details/gtrjsynoe.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.yfazqb.com/Article/details/gkldadnlk.sHtML

[R46] 递归替换文件内容
来源：http://www.share.vehdjk.com/Article/details/ganiagkqa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.bbcook.cn/Article/details/grgipxjgy.sHtML

[R47] sed 单行替换
来源：http://www.blog.tarul.cn/Article/details/gqprzpejd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gmodkbfrz.sHtML

[R48] awk 取指定列
来源：http://baike.tarul.cn/Article/details/gqaozyvfo.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.yfazqb.com/Article/details/grvlxxkxa.sHtML

[R49] awk 带条件
来源：http://www.share.epnwcf.com/Article/details/gwudnbpsn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.bbcook.cn/Article/details/ghwdifpwh.sHtML

[R50] awk 求和
来源：http://m.share.fktsv.cn/Article/details/gappbaasi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/ggieoqviu.sHtML

[R51] 排序去重取前几
来源：http://m.share.epnwcf.com/Article/details/gupbyatzr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.sjlbkw.cn/Article/details/gdjpbcrvy.sHtML

[R52] 统计行数
来源：http://mobile.fktsv.cn/Article/details/gqtgbbxmo.sHtML

wc -l a.txt
来源：http://mobile.epnwcf.com/Article/details/gwwbnmwng.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fktsv.cn/Article/details/gxkldwiee.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.sjlbkw.cn/Article/details/gbyrhfsqo.sHtML

[R54] 比较两个文件
来源：http://m.share.fktsv.cn/Article/details/guvaukagx.sHtML

diff a.txt b.txt
来源：http://m.share.bbcook.cn/Article/details/govatcmeq.sHtML

[R55] 压缩与解压
来源：http://wap.yfazqb.com/Article/details/gwiyrbjrh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.yfazqb.com/Article/details/gqcmnajtv.sHtML

[R56] 远程拷贝
来源：http://baike.fktsv.cn/Article/details/gtirdvxew.sHtML

scp file user@host:/path/
来源：http://wap.bbcook.cn/Article/details/gbdgesbka.sHtML

[R57] 远程执行命令
来源：http://www.share.bbcook.cn/Article/details/gfivwhsgc.sHtML

ssh user@host 'uptime'
来源：http://read.share.sjlbkw.cn/Article/details/gpjeufork.sHtML

[R58] 下载文件
来源：http://3g.tarul.cn/Article/details/gzeslspqv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.tarul.cn/Article/details/gpnchnsgy.sHtML

[R59] 发 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/gewhhmrzn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.bbcook.cn/Article/details/ghbdxsacm.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/gyrzgtdcl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.vehdjk.com/Article/details/grhgumvfj.sHtML

[R61] 磁盘占用
来源：http://www.share.fktsv.cn/Article/details/gomqzapfv.sHtML

df -h;  du -sh *
来源：http://baike.vehdjk.com/Article/details/gunqihwcz.sHtML

[R62] 找最占空间的文件
来源：http://www.share.yfazqb.com/Article/details/gyqzvhmxm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.epnwcf.com/Article/details/gednmyegu.sHtML

[R63] 内存与进程
来源：http://www.m.share.fktsv.cn/Article/details/gwaixelsy.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.sjlbkw.cn/Article/details/gwrfavmhd.sHtML

[R64] 结束进程
来源：http://wap.bbcook.cn/Article/details/gzdevatfs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.vehdjk.com/Article/details/gehiuwroh.sHtML

[R65] 查看端口占用
来源：http://mobile.fktsv.cn/Article/details/gkqunmhmf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.epnwcf.com/Article/details/ggajvbycm.sHtML

[R66] 定时任务
来源：http://www.blog.tarul.cn/Article/details/gtqofcseo.sHtML

crontab -e;  crontab -l
来源：http://www.blog.tarul.cn/Article/details/gqdxkhxhu.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.vehdjk.com/Article/details/gosxgnobc.sHtML

openssl rand -hex 16
来源：http://www.share.tarul.cn/Article/details/gloeeenns.sHtML

[R68] 计算文件校验值
来源：http://baike.tarul.cn/Article/details/gcdqrvdrc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gvocwrgfp.sHtML

[R69] 生成随机密码
来源：http://read.share.sjlbkw.cn/Article/details/glbqibilc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.bbcook.cn/Article/details/gsoraxacw.sHtML

[R70] 时间戳与互转
来源：http://www.blog.tarul.cn/Article/details/gdrscmyft.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.bbcook.cn/Article/details/gdlueutre.sHtML

[R71] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/glgxmxyqt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.epnwcf.com/Article/details/gqklekebp.sHtML

[R72] 等待端口就绪
来源：http://www.share.fktsv.cn/Article/details/gjbjvvbiv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.vehdjk.com/Article/details/gsndmzuzp.sHtML

[R73] 分割大日志
来源：http://mobile.bbcook.cn/Article/details/gqmwvtocf.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fktsv.cn/Article/details/gnerppvbl.sHtML

[R74] 批量重命名
来源：http://www.share.vehdjk.com/Article/details/gvpfpkuec.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.sjlbkw.cn/Article/details/gzqajmpeb.sHtML

[R75] 导出环境变量
来源：http://baike.vehdjk.com/Article/details/ghfmitytq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.yfazqb.com/Article/details/ghkmfqsxk.sHtML

[R76] 使用临时文件
来源：http://wap.bbcook.cn/Article/details/gfcnjdlxz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/ggtgnrbsl.sHtML

[R77] 读取用户输入
来源：http://baike.fktsv.cn/Article/details/gckfxbcjn.sHtML

read -rp "请输入: " ans
来源：http://read.share.epnwcf.com/Article/details/gemwaiyhw.sHtML

[R78] 交互式菜单
来源：http://www.m.share.vehdjk.com/Article/details/grfxxgbtq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.epnwcf.com/Article/details/gjustbuou.sHtML

[R79] 解析命令行选项
来源：http://3g.bbcook.cn/Article/details/gpabuexgv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.epnwcf.com/Article/details/gltrqakkr.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.tarul.cn/Article/details/ghytbfxpt.sHtML

time ./run.sh
来源：http://mobile.bbcook.cn/Article/details/gbpkdonro.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gnthsbfzt.sHtML

S. C / C++ 专题
来源：http://wap.tarul.cn/Article/details/gbrhjqldc.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gfrigqxgt.sHtML

[S01] C：Hello World
来源：http://m.share.yfazqb.com/Article/details/gqwoshsjz.sHtML

#include <stdio.h>
来源：http://www.m.share.yfazqb.com/Article/details/gcbianfki.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.sjlbkw.cn/Article/details/gvjxyfqbr.sHtML

[S02] C：变量与格式化输出
来源：http://baike.vehdjk.com/Article/details/goeawugib.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.bbcook.cn/Article/details/gfuhlgyjw.sHtML

[S03] C：读入整数
来源：http://read.share.fktsv.cn/Article/details/guwlwvykn.sHtML

int x; scanf("%d", &x);
来源：http://3g.tarul.cn/Article/details/glbxkezfm.sHtML

[S04] C：字符串复制
来源：http://baike.epnwcf.com/Article/details/glkfulilj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.bbcook.cn/Article/details/gizsbowoq.sHtML

[S05] C：字符串长度
来源：http://3g.yfazqb.com/Article/details/gopbhmnqu.sHtML

strlen(s)
来源：http://mobile.sjlbkw.cn/Article/details/gpkunvoje.sHtML

[S06] C：字符串比较
来源：http://www.m.share.vehdjk.com/Article/details/gjyszzplu.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.tarul.cn/Article/details/garmwrmiv.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fktsv.cn/Article/details/gekueqpeg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.yfazqb.com/Article/details/gfdaswkuw.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fktsv.cn/Article/details/gzjgabusr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.bbcook.cn/Article/details/grmhteltl.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.yfazqb.com/Article/details/gcmmhykif.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.sjlbkw.cn/Article/details/ghehlmutu.sHtML

[S10] C：指针与解引用
来源：http://www.blog.vehdjk.com/Article/details/gjpvwlyra.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.epnwcf.com/Article/details/giugulkjs.sHtML

[S11] C：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gzvjigyts.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.bbcook.cn/Article/details/ggvshdpky.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fktsv.cn/Article/details/gtoszymfj.sHtML

fclose(f);
来源：http://m.share.tarul.cn/Article/details/gkvwvecdb.sHtML

[S12] C：写文件
来源：http://mobile.tarul.cn/Article/details/glolkbxvq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/gsqfoysrr.sHtML

[S13] C：宏定义
来源：http://wap.sjlbkw.cn/Article/details/gzuqgtgtq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.epnwcf.com/Article/details/gbchsdgpv.sHtML

[S14] C：枚举
来源：http://read.share.bbcook.cn/Article/details/gggyjrfff.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.yfazqb.com/Article/details/gkjxlqghq.sHtML

[S15] C：类型转换
来源：http://www.blog.vehdjk.com/Article/details/gvjjdxddw.sHtML

(double) a / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gejlqwbxq.sHtML

[S16] C：位操作置位
来源：http://3g.sjlbkw.cn/Article/details/glkuzzfhp.sHtML

x |= (1 << 3);
来源：http://wap.fktsv.cn/Article/details/gzqebicxq.sHtML

[S17] C：安全拼接字符串
来源：http://3g.epnwcf.com/Article/details/gyrhzdqex.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.vehdjk.com/Article/details/gwuoinsbb.sHtML

[S18] C：命令行参数
来源：http://wap.fktsv.cn/Article/details/gzafhnbvc.sHtML

int main(int argc, char **argv)
来源：http://www.blog.tarul.cn/Article/details/gvvhizicj.sHtML

[S19] C：快速排序
来源：http://blog.vehdjk.com/Article/details/guvavfzii.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/gijfxczzi.sHtML

[S20] C：二分查找
来源：http://3g.epnwcf.com/Article/details/gdurkxazr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gavrfvqho.sHtML

[S21] C：字符类别判断
来源：http://blog.bbcook.cn/Article/details/gezknnupm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.sjlbkw.cn/Article/details/gccfiuimv.sHtML

[S22] C：字符串转数字
来源：http://www.blog.bbcook.cn/Article/details/gxuoyrwdp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fktsv.cn/Article/details/glessickh.sHtML

[S23] C：随机数
来源：http://www.blog.epnwcf.com/Article/details/gdyiqqwab.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.bbcook.cn/Article/details/gfvbzyjhr.sHtML

[S24] C：获取本地时间
来源：http://wap.bbcook.cn/Article/details/gjmlykolc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.bbcook.cn/Article/details/gqtyadvyp.sHtML

[S25] C：内存拷贝
来源：http://mobile.epnwcf.com/Article/details/gsenrsfgj.sHtML

memcpy(dst, src, n);
来源：http://www.share.fktsv.cn/Article/details/givcgvtii.sHtML

[S26] C：内存清零
来源：http://3g.vehdjk.com/Article/details/gfaorqonl.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/gtjwvbfgp.sHtML

[S27] C：定义常量
来源：http://m.share.vehdjk.com/Article/details/gxpqsqowm.sHtML

const double PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/grzbfoqjs.sHtML

[S28] C：静态变量
来源：http://www.blog.vehdjk.com/Article/details/gntepkeqm.sHtML

static int counter = 0;
来源：http://www.m.share.fktsv.cn/Article/details/glyzdkpwh.sHtML

[S29] C：变参函数
来源：http://3g.sjlbkw.cn/Article/details/gtwdnszth.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.sjlbkw.cn/Article/details/gbqplrlhh.sHtML

[S30] C：头文件保护
来源：http://mobile.fktsv.cn/Article/details/gzzkjeraw.sHtML

#ifndef X_H
来源：http://wap.vehdjk.com/Article/details/gtnidrypd.sHtML

#define X_H
来源：http://3g.bbcook.cn/Article/details/gfeequovy.sHtML

#endif
来源：http://www.m.share.fktsv.cn/Article/details/gpquwayuq.sHtML

[S31] C++：Hello World
来源：http://m.share.bbcook.cn/Article/details/glernzkcv.sHtML

#include <iostream>
来源：http://baike.sjlbkw.cn/Article/details/gecpswesl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fktsv.cn/Article/details/gtnhukjfi.sHtML

[S32] C++：字符串
来源：http://m.share.epnwcf.com/Article/details/gyedmnevx.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.tarul.cn/Article/details/gwpgagnmr.sHtML

[S33] C++：vector 增删
来源：http://wap.epnwcf.com/Article/details/giiwxfuyr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fktsv.cn/Article/details/gedagmbmy.sHtML

[S34] C++：遍历 vector
来源：http://read.share.sjlbkw.cn/Article/details/gihudlsqj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/gedxdgssz.sHtML


<!-- 参考信息 -->