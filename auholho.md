代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.tarul.cn/Article/details/gkegujqig.sHtML

[Q52] 删除指定行
来源：http://mobile.tarul.cn/Article/details/gslneriuv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gahnzdnfa.sHtML

[Q53] 按条件删除
来源：http://mobile.epnwcf.com/Article/details/garsfiuyk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.sjlbkw.cn/Article/details/gvvdxmmiv.sHtML

[Q54] 清空表
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdmwjnhp.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.tarul.cn/Article/details/gpdxvpiit.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fktsv.cn/Article/details/gdotrjmcv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.yfazqb.com/Article/details/gdybxztqi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.bbcook.cn/Article/details/gwoniyhzd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gffezolzu.sHtML

[Q57] 行号
来源：http://mobile.vehdjk.com/Article/details/ghxafbnbi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.tarul.cn/Article/details/gfcnkstac.sHtML

[Q58] 累计求和
来源：http://wap.yfazqb.com/Article/details/gjzzkpvsb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.bbcook.cn/Article/details/gpaorakkv.sHtML

[Q59] 分组内累计
来源：http://mobile.epnwcf.com/Article/details/gqqwfhkjn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gfvzxjlvk.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.sjlbkw.cn/Article/details/gemkerzaa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkkgvgjg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gxfrlvtiu.sHtML

[Q61] 移动平均
来源：http://blog.tarul.cn/Article/details/gcaqtigth.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gpgeofmlp.sHtML

[Q62] 分组占比
来源：http://www.blog.sjlbkw.cn/Article/details/gyfmzvzpf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/gfbvggaem.sHtML

[Q63] 开启事务
来源：http://baike.tarul.cn/Article/details/gllrmmbxg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.yfazqb.com/Article/details/gjzywvauo.sHtML

[Q64] 提交事务
来源：http://www.blog.sjlbkw.cn/Article/details/gwaajdnga.sHtML

COMMIT;
来源：http://mobile.sjlbkw.cn/Article/details/gqltsibzu.sHtML

[Q65] 回滚事务
来源：http://www.share.sjlbkw.cn/Article/details/gdshtfdqm.sHtML

ROLLBACK;
来源：http://m.share.bbcook.cn/Article/details/gemtetgam.sHtML

[Q66] 行锁查询
来源：http://baike.tarul.cn/Article/details/gmrlhmbxi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.tarul.cn/Article/details/geaupzili.sHtML

[Q67] 设置隔离级别
来源：http://mobile.bbcook.cn/Article/details/gedzltpow.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.bbcook.cn/Article/details/ghbyporuu.sHtML

[Q68] 保存点
来源：http://read.share.fktsv.cn/Article/details/gzwtcgeez.sHtML

SAVEPOINT sp1;
来源：http://www.blog.tarul.cn/Article/details/gktawmppo.sHtML

ROLLBACK TO sp1;
来源：http://read.share.bbcook.cn/Article/details/glgfthdns.sHtML

[Q69] 查看执行计划
来源：http://3g.yfazqb.com/Article/details/gpcntgqxp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fktsv.cn/Article/details/gbfqdacpw.sHtML

[Q70] 更新统计信息
来源：http://mobile.fktsv.cn/Article/details/gfhpgslmz.sHtML

ANALYZE TABLE users;
来源：http://3g.bbcook.cn/Article/details/gmtgcycax.sHtML

[Q71] 查看建表语句
来源：http://3g.fktsv.cn/Article/details/gzdbmwozr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.vehdjk.com/Article/details/gpvackxis.sHtML

[Q72] 查看索引
来源：http://3g.epnwcf.com/Article/details/goglueqqe.sHtML

SHOW INDEX FROM users;
来源：http://www.share.tarul.cn/Article/details/gkofgoiih.sHtML

[Q73] 查看表状态
来源：http://read.share.sjlbkw.cn/Article/details/gdcnqdfdl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.epnwcf.com/Article/details/ggtwaepwi.sHtML

[Q74] 强制使用索引
来源：http://www.share.yfazqb.com/Article/details/gmkbuwzxf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.vehdjk.com/Article/details/gahjfvdtr.sHtML

[Q75] 日期格式化
来源：http://m.share.tarul.cn/Article/details/grlwghyhl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gqqppfcuu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.tarul.cn/Article/details/gdzlwekqa.sHtML

[Q76] 按天统计
来源：http://www.share.tarul.cn/Article/details/giijbheiq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.bbcook.cn/Article/details/gbhiahygo.sHtML

[Q77] 时间加减
来源：http://m.share.sjlbkw.cn/Article/details/gpsztgaac.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.tarul.cn/Article/details/gwlojvtlb.sHtML

[Q78] 当前时间
来源：http://www.blog.yfazqb.com/Article/details/gvkmikots.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.yfazqb.com/Article/details/gmbmiyzaj.sHtML

[Q79] 字符串拼接
来源：http://read.share.vehdjk.com/Article/details/gbhxkcjan.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.yfazqb.com/Article/details/glrnrmfrr.sHtML

[Q80] 字符串截取
来源：http://3g.sjlbkw.cn/Article/details/gdcgoqdpj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fktsv.cn/Article/details/glzpwgmxx.sHtML

[Q81] 字符串替换
来源：http://m.share.vehdjk.com/Article/details/glfxplqop.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.epnwcf.com/Article/details/gyyseixog.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fktsv.cn/Article/details/giwlzoxlm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gfahnuyzc.sHtML

[Q83] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gbjrvxhnw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gtsokvcmw.sHtML

[Q84] 去除首尾空格
来源：http://mobile.sjlbkw.cn/Article/details/giepmaenm.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/gjogbxmle.sHtML

[Q85] 数值取整
来源：http://www.blog.tarul.cn/Article/details/gvgyptykf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.tarul.cn/Article/details/gefmpukby.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.yfazqb.com/Article/details/gipzyrwif.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.vehdjk.com/Article/details/gqjbmsaaj.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.bbcook.cn/Article/details/gqobpyaij.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.tarul.cn/Article/details/gryrpjwxa.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fktsv.cn/Article/details/gizamxqkx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.bbcook.cn/Article/details/ggvzukgoe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.vehdjk.com/Article/details/gzdaxqojd.sHtML

[Q89] 判断表是否存在
来源：http://m.share.epnwcf.com/Article/details/gzzzhhswy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fktsv.cn/Article/details/gevewujnc.sHtML

[Q90] 生成序号列
来源：http://www.m.share.sjlbkw.cn/Article/details/gavafngso.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.bbcook.cn/Article/details/gwuublusl.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gwqrsszdt.sHtML

R. Bash 专题
来源：http://www.m.share.tarul.cn/Article/details/gzgtjqpuv.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gbvogmukf.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.tarul.cn/Article/details/guujqezih.sHtML

#!/usr/bin/env bash
来源：http://baike.yfazqb.com/Article/details/gpvctilga.sHtML

set -euo pipefail
来源：http://www.m.share.epnwcf.com/Article/details/glolliueb.sHtML

[R02] 变量赋值与使用
来源：http://mobile.epnwcf.com/Article/details/gfxmxdhmb.sHtML

name="Tom"; echo "$name"
来源：http://3g.fktsv.cn/Article/details/gswnxvckx.sHtML

[R03] 只读变量
来源：http://www.blog.epnwcf.com/Article/details/gqqpvvqnb.sHtML

readonly PI=3.14
来源：http://3g.sjlbkw.cn/Article/details/godhksojg.sHtML

[R04] 位置参数
来源：http://blog.epnwcf.com/Article/details/glnbwzsli.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fktsv.cn/Article/details/gcukkeqja.sHtML

[R05] 参数默认值
来源：http://m.share.fktsv.cn/Article/details/gvowelknq.sHtML

name="${1:-default}"
来源：http://www.blog.fktsv.cn/Article/details/gwzvvqbpv.sHtML

[R06] 判断命令是否存在
来源：http://blog.bbcook.cn/Article/details/gmgggenpj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/gosvmsivn.sHtML

[R07] if 判断文件
来源：http://blog.bbcook.cn/Article/details/gwsghlhzl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.bbcook.cn/Article/details/geyzykasp.sHtML

[R08] 数值比较
来源：http://www.m.share.yfazqb.com/Article/details/gxpfphrcq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gujyccwku.sHtML

[R09] 字符串比较
来源：http://m.share.bbcook.cn/Article/details/gxmdlagvs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fktsv.cn/Article/details/ggeihbyce.sHtML

[R10] 正则匹配
来源：http://www.m.share.yfazqb.com/Article/details/ghsbevmhy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.tarul.cn/Article/details/gdvyyxvck.sHtML

[R11] case 多分支
来源：http://www.blog.tarul.cn/Article/details/gpndxkbog.sHtML

case "$1" in
来源：http://3g.yfazqb.com/Article/details/gsuopblop.sHtML

start) echo "启动" ;;
来源：http://www.blog.bbcook.cn/Article/details/gowyloumj.sHtML

stop)  echo "停止" ;;
来源：http://www.share.yfazqb.com/Article/details/gbytlluku.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.vehdjk.com/Article/details/gtuqkyqgf.sHtML

esac
来源：http://www.share.vehdjk.com/Article/details/gwmelvnfg.sHtML

[R12] for 遍历文件
来源：http://m.share.bbcook.cn/Article/details/gukqhhvrk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.sjlbkw.cn/Article/details/gbijfsrcs.sHtML

[R13] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/gmwayvgie.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.tarul.cn/Article/details/gptamnroa.sHtML

[R14] C 风格 for
来源：http://3g.tarul.cn/Article/details/gbhffdzru.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/gamaxjjid.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gogfqkndr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.yfazqb.com/Article/details/gsvnlkgoc.sHtML

[R16] until 等待条件
来源：http://read.share.epnwcf.com/Article/details/ggwwiojsz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.tarul.cn/Article/details/grrsqzdxd.sHtML

[R17] 数组定义与取值
来源：http://www.share.epnwcf.com/Article/details/gtzdknsmg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.epnwcf.com/Article/details/glmlsjabv.sHtML

[R18] 遍历数组
来源：http://mobile.tarul.cn/Article/details/gmflbcpwk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.vehdjk.com/Article/details/gywbrzdzb.sHtML

[R19] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/gsozfxgtt.sHtML

echo "${#arr[@]}"
来源：http://m.share.bbcook.cn/Article/details/gnijdeufb.sHtML

[R20] 关联数组（字典）
来源：http://mobile.vehdjk.com/Article/details/gvfuagyfo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.bbcook.cn/Article/details/gehrtduwk.sHtML

[R21] 字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gefsseejq.sHtML

echo "${#s}"
来源：http://mobile.bbcook.cn/Article/details/giflqyjxf.sHtML

[R22] 截取子串
来源：http://www.blog.tarul.cn/Article/details/ggsnhgasu.sHtML

echo "${s:0:5}"
来源：http://mobile.epnwcf.com/Article/details/gnoxpxxvy.sHtML

[R23] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/gjlnarnyw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.vehdjk.com/Article/details/gcxzkjkyg.sHtML

[R24] 大小写转换
来源：http://3g.sjlbkw.cn/Article/details/gbarwwmcp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.yfazqb.com/Article/details/gdtgobxxi.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.vehdjk.com/Article/details/gomszulcf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.bbcook.cn/Article/details/glofxuzwc.sHtML

[R26] 命令替换
来源：http://read.share.vehdjk.com/Article/details/gomipfbvt.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.sjlbkw.cn/Article/details/gtjiwrzyy.sHtML

[R27] 算术展开
来源：http://wap.tarul.cn/Article/details/gxipdegsf.sHtML

echo $((1 + 2 * 3))
来源：http://baike.yfazqb.com/Article/details/gqjzoqsgv.sHtML

[R28] 浮点运算
来源：http://read.share.vehdjk.com/Article/details/gykrjemuz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvigpjwa.sHtML

[R29] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/gilyxzoen.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.tarul.cn/Article/details/gpohtsumy.sHtML

[R30] 函数返回状态码
来源：http://www.blog.tarul.cn/Article/details/gfnithvqv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.yfazqb.com/Article/details/ghxdvptvb.sHtML

[R31] 局部变量
来源：http://m.share.tarul.cn/Article/details/gmbnazlov.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fktsv.cn/Article/details/gndoececl.sHtML

[R32] 参数个数校验
来源：http://3g.tarul.cn/Article/details/gpigastbz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/gdirrakib.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.bbcook.cn/Article/details/gbcpnzoif.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.vehdjk.com/Article/details/gvwwrvtyt.sHtML

[R34] 退出时清理
来源：http://www.share.bbcook.cn/Article/details/gpxyrnvgg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/gufobqvbm.sHtML

[R35] 后台执行并等待
来源：http://3g.tarul.cn/Article/details/gorqhtipb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/ghrbvsfav.sHtML

[R36] 并发执行多个任务
来源：http://blog.tarul.cn/Article/details/gulmvolwp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.epnwcf.com/Article/details/gvfkqncvc.sHtML

[R37] 把输出赋给变量
来源：http://www.share.bbcook.cn/Article/details/gmvhoibuz.sHtML

files=$(ls -1)
来源：http://www.share.sjlbkw.cn/Article/details/ghcgwrnyh.sHtML

[R38] 管道串联
来源：http://read.share.sjlbkw.cn/Article/details/ghfjzzvgi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.epnwcf.com/Article/details/gqytlkbcz.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.sjlbkw.cn/Article/details/gywbuuydd.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fktsv.cn/Article/details/geqesgcli.sHtML

[R40] 追加写日志
来源：http://3g.epnwcf.com/Article/details/gdmsjdgoa.sHtML

echo "log" >> out.log
来源：http://wap.vehdjk.com/Article/details/gimirpinx.sHtML

[R41] 丢弃输出
来源：http://www.blog.tarul.cn/Article/details/gxgjwwuee.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fktsv.cn/Article/details/gdltjxaez.sHtML

[R42] 输入重定向
来源：http://mobile.yfazqb.com/Article/details/gsofnhihi.sHtML

wc -l < a.txt
来源：http://read.share.bbcook.cn/Article/details/glbazvfhz.sHtML

[R43] 按名字查找文件
来源：http://mobile.epnwcf.com/Article/details/gmiatpcev.sHtML

find . -name "*.log" -type f
来源：http://www.share.fktsv.cn/Article/details/ghfgbjetm.sHtML

[R44] 按修改时间查找
来源：http://www.share.yfazqb.com/Article/details/gduovtfyh.sHtML

find . -mtime -7 -type f
来源：http://blog.epnwcf.com/Article/details/gxuvqiesq.sHtML

[R45] 批量删除
来源：http://www.m.share.tarul.cn/Article/details/gdcmczcwb.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.tarul.cn/Article/details/gacfwrwbl.sHtML

[R46] 递归替换文件内容
来源：http://wap.vehdjk.com/Article/details/grmpvuvfz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.sjlbkw.cn/Article/details/gifkfjegj.sHtML

[R47] sed 单行替换
来源：http://baike.yfazqb.com/Article/details/gdohououc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gladvmsrn.sHtML

[R48] awk 取指定列
来源：http://www.share.fktsv.cn/Article/details/gntrwykmy.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fktsv.cn/Article/details/gkuruuxkz.sHtML

[R49] awk 带条件
来源：http://wap.epnwcf.com/Article/details/gstqsscqd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.tarul.cn/Article/details/gwvumivyk.sHtML

[R50] awk 求和
来源：http://mobile.epnwcf.com/Article/details/gvpymgrlv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.yfazqb.com/Article/details/gwvlycxps.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.yfazqb.com/Article/details/gnrertsmd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.yfazqb.com/Article/details/gsmqhiunk.sHtML

[R52] 统计行数
来源：http://mobile.vehdjk.com/Article/details/gsmlagpzx.sHtML

wc -l a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gkanpppdi.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.yfazqb.com/Article/details/ggidqmrmt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.yfazqb.com/Article/details/ggekbzvcm.sHtML

[R54] 比较两个文件
来源：http://www.share.tarul.cn/Article/details/gvugchufj.sHtML

diff a.txt b.txt
来源：http://www.blog.vehdjk.com/Article/details/gaoqsbrjg.sHtML

[R55] 压缩与解压
来源：http://wap.fktsv.cn/Article/details/gdbjhtniy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.sjlbkw.cn/Article/details/gxamfttgy.sHtML

[R56] 远程拷贝
来源：http://www.blog.yfazqb.com/Article/details/gititnbmo.sHtML

scp file user@host:/path/
来源：http://wap.epnwcf.com/Article/details/ghobhiyix.sHtML

[R57] 远程执行命令
来源：http://www.share.yfazqb.com/Article/details/gygywzorh.sHtML

ssh user@host 'uptime'
来源：http://www.blog.tarul.cn/Article/details/giavappfy.sHtML

[R58] 下载文件
来源：http://baike.yfazqb.com/Article/details/gghohpowy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.yfazqb.com/Article/details/gskjrsvda.sHtML

[R59] 发 POST JSON
来源：http://3g.vehdjk.com/Article/details/ghoylezpy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.sjlbkw.cn/Article/details/gkocuczbz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.tarul.cn/Article/details/gpndiowpu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.tarul.cn/Article/details/glfzecchs.sHtML

[R61] 磁盘占用
来源：http://mobile.yfazqb.com/Article/details/ggvaeddjj.sHtML

df -h;  du -sh *
来源：http://wap.vehdjk.com/Article/details/godduwckz.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.tarul.cn/Article/details/guqqbervw.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.yfazqb.com/Article/details/gkvjitnyn.sHtML

[R63] 内存与进程
来源：http://www.blog.sjlbkw.cn/Article/details/gizsqxxdw.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.tarul.cn/Article/details/gltcmxsov.sHtML

[R64] 结束进程
来源：http://baike.bbcook.cn/Article/details/ggdonzrwf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.tarul.cn/Article/details/gywrwkwdv.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fktsv.cn/Article/details/gdqjbcuxl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.yfazqb.com/Article/details/gvgfjnmwu.sHtML

[R66] 定时任务
来源：http://www.blog.bbcook.cn/Article/details/golpdzckz.sHtML

crontab -e;  crontab -l
来源：http://www.share.fktsv.cn/Article/details/gwarxlmkk.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fktsv.cn/Article/details/gkxvfacen.sHtML

openssl rand -hex 16
来源：http://m.share.tarul.cn/Article/details/guqyljwhg.sHtML

[R68] 计算文件校验值
来源：http://www.share.epnwcf.com/Article/details/gtsadpvow.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.tarul.cn/Article/details/gwenmxoxz.sHtML

[R69] 生成随机密码
来源：http://m.share.sjlbkw.cn/Article/details/gikudmhcq.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.vehdjk.com/Article/details/grfbkquyc.sHtML

[R70] 时间戳与互转
来源：http://read.share.fktsv.cn/Article/details/guazsswiv.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.tarul.cn/Article/details/glakcwxoq.sHtML

[R71] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gubplstkf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.epnwcf.com/Article/details/glnlytksr.sHtML

[R72] 等待端口就绪
来源：http://www.blog.bbcook.cn/Article/details/gkjuchxhr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/gsdnwstru.sHtML

[R73] 分割大日志
来源：http://wap.sjlbkw.cn/Article/details/gnbdvjpsi.sHtML

split -l 1000 big.log part_
来源：http://www.blog.yfazqb.com/Article/details/gilzxtnxq.sHtML

[R74] 批量重命名
来源：http://mobile.sjlbkw.cn/Article/details/gmhpfsfxj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.yfazqb.com/Article/details/gopxufxpk.sHtML

[R75] 导出环境变量
来源：http://www.blog.fktsv.cn/Article/details/gwmnkpqnv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.yfazqb.com/Article/details/gratxjzdx.sHtML

[R76] 使用临时文件
来源：http://blog.yfazqb.com/Article/details/gfqjoavqy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fktsv.cn/Article/details/ggoednxjm.sHtML

[R77] 读取用户输入
来源：http://3g.vehdjk.com/Article/details/ggyrillhf.sHtML

read -rp "请输入: " ans
来源：http://mobile.epnwcf.com/Article/details/gyeogftzh.sHtML

[R78] 交互式菜单
来源：http://baike.sjlbkw.cn/Article/details/gobnffvao.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.vehdjk.com/Article/details/gquuavdof.sHtML

[R79] 解析命令行选项
来源：http://wap.vehdjk.com/Article/details/gtbnvqsmc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fktsv.cn/Article/details/gnlefklfu.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.vehdjk.com/Article/details/gzfmrbaze.sHtML

time ./run.sh
来源：http://www.blog.yfazqb.com/Article/details/gylbfbdgf.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ghtkgtddk.sHtML

S. C / C++ 专题
来源：http://mobile.yfazqb.com/Article/details/gfnfwwhyt.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/grlpmusxg.sHtML

[S01] C：Hello World
来源：http://m.share.fktsv.cn/Article/details/gcrydwwru.sHtML

#include <stdio.h>
来源：http://3g.yfazqb.com/Article/details/gmvaxhwkh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.sjlbkw.cn/Article/details/gryouunmu.sHtML

[S02] C：变量与格式化输出
来源：http://blog.epnwcf.com/Article/details/gswdqxlwh.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.epnwcf.com/Article/details/gkhekxrzw.sHtML

[S03] C：读入整数
来源：http://www.blog.sjlbkw.cn/Article/details/gezwvyhvn.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.vehdjk.com/Article/details/gicmderfo.sHtML

[S04] C：字符串复制
来源：http://wap.bbcook.cn/Article/details/gmsvhlwls.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.vehdjk.com/Article/details/gpycxdbtp.sHtML

[S05] C：字符串长度
来源：http://baike.vehdjk.com/Article/details/gnvbxkkun.sHtML

strlen(s)
来源：http://blog.fktsv.cn/Article/details/gafhceiqo.sHtML

[S06] C：字符串比较
来源：http://blog.fktsv.cn/Article/details/gxwcfucty.sHtML

strcmp(a, b) == 0
来源：http://www.share.fktsv.cn/Article/details/gnuishpmd.sHtML

[S07] C：数组遍历求和
来源：http://m.share.tarul.cn/Article/details/gxwyctyyc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.bbcook.cn/Article/details/gghzjmujm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fktsv.cn/Article/details/gicprltgn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmatvbjm.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.tarul.cn/Article/details/ghbeumusw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.sjlbkw.cn/Article/details/gxdfxzmol.sHtML

[S10] C：指针与解引用
来源：http://blog.tarul.cn/Article/details/gtxbfzslp.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.vehdjk.com/Article/details/glbfxzsph.sHtML

[S11] C：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gjsxanjxs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.yfazqb.com/Article/details/glgvqguhq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.vehdjk.com/Article/details/gmgcrzpxw.sHtML

fclose(f);
来源：http://blog.sjlbkw.cn/Article/details/gsptaastm.sHtML

[S12] C：写文件
来源：http://3g.fktsv.cn/Article/details/giyulcfvk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/gktqxraqf.sHtML

[S13] C：宏定义
来源：http://www.blog.vehdjk.com/Article/details/gyrkqvwmo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.bbcook.cn/Article/details/gvjdpvxtc.sHtML

[S14] C：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gqorqbvuj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.bbcook.cn/Article/details/gyxdwptml.sHtML

[S15] C：类型转换
来源：http://www.m.share.bbcook.cn/Article/details/gyeqhorkz.sHtML

(double) a / b
来源：http://www.blog.vehdjk.com/Article/details/gsfztzxju.sHtML

[S16] C：位操作置位
来源：http://wap.bbcook.cn/Article/details/gsccmhiwl.sHtML

x |= (1 << 3);
来源：http://www.share.sjlbkw.cn/Article/details/gfsbiztpu.sHtML

[S17] C：安全拼接字符串
来源：http://blog.vehdjk.com/Article/details/gbhoishgk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.tarul.cn/Article/details/gfpdkbuuv.sHtML

[S18] C：命令行参数
来源：http://baike.fktsv.cn/Article/details/gfgyhvgqa.sHtML

int main(int argc, char **argv)
来源：http://www.share.fktsv.cn/Article/details/glaldhgkq.sHtML

[S19] C：快速排序
来源：http://baike.sjlbkw.cn/Article/details/gahjsxdao.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/gwsldmzge.sHtML

[S20] C：二分查找
来源：http://www.blog.epnwcf.com/Article/details/gijdyypuv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.epnwcf.com/Article/details/ginzufdhs.sHtML

[S21] C：字符类别判断
来源：http://baike.fktsv.cn/Article/details/gcpoyhvjy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.bbcook.cn/Article/details/geecbsmpc.sHtML

[S22] C：字符串转数字
来源：http://www.share.yfazqb.com/Article/details/ggktopgue.sHtML


<!-- 参考信息 -->