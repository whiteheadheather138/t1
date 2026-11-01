代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.bbcook.cn/Article/details/geywzyrxz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzhhnqvo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/grfackksy.sHtML

[Q57] 行号
来源：http://mobile.sjlbkw.cn/Article/details/grlyjtqlc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.tarul.cn/Article/details/gnflevicp.sHtML

[Q58] 累计求和
来源：http://www.share.fktsv.cn/Article/details/gleldcmjn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gqyfvnajs.sHtML

[Q59] 分组内累计
来源：http://www.share.tarul.cn/Article/details/gkvmezyix.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/garobfcmw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.yfazqb.com/Article/details/gtzlthfgh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.epnwcf.com/Article/details/gbxcoekfk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gixbymugi.sHtML

[Q61] 移动平均
来源：http://wap.fktsv.cn/Article/details/gpiwjxprq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gxsleisme.sHtML

[Q62] 分组占比
来源：http://3g.fktsv.cn/Article/details/glgnsqmbr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gipbkgkly.sHtML

[Q63] 开启事务
来源：http://wap.fktsv.cn/Article/details/gqqgxxpfw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/gajocojah.sHtML

[Q64] 提交事务
来源：http://www.blog.epnwcf.com/Article/details/gyldcqeni.sHtML

COMMIT;
来源：http://mobile.tarul.cn/Article/details/gqthutpsq.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fktsv.cn/Article/details/gyzkrxrrx.sHtML

ROLLBACK;
来源：http://www.m.share.vehdjk.com/Article/details/ggarcznni.sHtML

[Q66] 行锁查询
来源：http://read.share.tarul.cn/Article/details/geqvvfdgv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.epnwcf.com/Article/details/gtiqpjgcm.sHtML

[Q67] 设置隔离级别
来源：http://wap.bbcook.cn/Article/details/gseiggfnz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.tarul.cn/Article/details/gdsjgelpp.sHtML

[Q68] 保存点
来源：http://www.m.share.vehdjk.com/Article/details/gdvcljthn.sHtML

SAVEPOINT sp1;
来源：http://read.share.tarul.cn/Article/details/gnfwricpj.sHtML

ROLLBACK TO sp1;
来源：http://m.share.vehdjk.com/Article/details/gadwrtuoq.sHtML

[Q69] 查看执行计划
来源：http://www.share.sjlbkw.cn/Article/details/gpydhblcu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.epnwcf.com/Article/details/gmqtacrry.sHtML

[Q70] 更新统计信息
来源：http://www.blog.vehdjk.com/Article/details/gzbjtqctr.sHtML

ANALYZE TABLE users;
来源：http://baike.vehdjk.com/Article/details/gszvikdwv.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fktsv.cn/Article/details/gjdeujnha.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.vehdjk.com/Article/details/gdiqxrrxe.sHtML

[Q72] 查看索引
来源：http://3g.tarul.cn/Article/details/gbrgyzpcr.sHtML

SHOW INDEX FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gbzpodzxz.sHtML

[Q73] 查看表状态
来源：http://baike.bbcook.cn/Article/details/ghbfrfxcm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.sjlbkw.cn/Article/details/gplsxxeik.sHtML

[Q74] 强制使用索引
来源：http://m.share.bbcook.cn/Article/details/gopivjyio.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fktsv.cn/Article/details/guaeakeyj.sHtML

[Q75] 日期格式化
来源：http://wap.tarul.cn/Article/details/glgpijkvz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.tarul.cn/Article/details/gwiaybdrx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fktsv.cn/Article/details/gzoyssgyr.sHtML

[Q76] 按天统计
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtoutvkq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.bbcook.cn/Article/details/gajuluuwe.sHtML

[Q77] 时间加减
来源：http://baike.vehdjk.com/Article/details/gzphkvegr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.vehdjk.com/Article/details/gznnspabl.sHtML

[Q78] 当前时间
来源：http://m.share.yfazqb.com/Article/details/gjnqhebtj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.vehdjk.com/Article/details/grsmzblkk.sHtML

[Q79] 字符串拼接
来源：http://blog.bbcook.cn/Article/details/gvxbvbzck.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.epnwcf.com/Article/details/gdzxwjxgq.sHtML

[Q80] 字符串截取
来源：http://www.m.share.yfazqb.com/Article/details/gmhtnaucd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gxbpznukc.sHtML

[Q81] 字符串替换
来源：http://blog.tarul.cn/Article/details/gzqeieouy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.vehdjk.com/Article/details/gsylxvopn.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.epnwcf.com/Article/details/gevwzkusv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gzumxumas.sHtML

[Q83] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/gvppvuqvk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gllvmrwcy.sHtML

[Q84] 去除首尾空格
来源：http://blog.tarul.cn/Article/details/gxhjdnxlk.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gzhcupgff.sHtML

[Q85] 数值取整
来源：http://www.m.share.bbcook.cn/Article/details/gkkfhlhue.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.yfazqb.com/Article/details/gxfxarwbo.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.sjlbkw.cn/Article/details/gxbocnnpy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fktsv.cn/Article/details/gxpaljdmc.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.tarul.cn/Article/details/ghifdslhe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.yfazqb.com/Article/details/gaorhvyyl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.vehdjk.com/Article/details/gqkntsecb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.tarul.cn/Article/details/gxxkfpiir.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.vehdjk.com/Article/details/gcjzkkxlw.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.bbcook.cn/Article/details/gdfmyozmc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.tarul.cn/Article/details/gqoakmwgx.sHtML

[Q90] 生成序号列
来源：http://wap.vehdjk.com/Article/details/gthbmfewq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.bbcook.cn/Article/details/ggleperyo.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gvbgiyziw.sHtML

R. Bash 专题
来源：http://baike.vehdjk.com/Article/details/gkszcnliv.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ggcfbvatq.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fktsv.cn/Article/details/gowtpbqfg.sHtML

#!/usr/bin/env bash
来源：http://mobile.vehdjk.com/Article/details/gmzwhwtyj.sHtML

set -euo pipefail
来源：http://www.share.yfazqb.com/Article/details/gbcwgkhgb.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.tarul.cn/Article/details/gpujuwovu.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fktsv.cn/Article/details/grhlywore.sHtML

[R03] 只读变量
来源：http://www.blog.bbcook.cn/Article/details/gbnaopuhw.sHtML

readonly PI=3.14
来源：http://wap.sjlbkw.cn/Article/details/gqhfowzql.sHtML

[R04] 位置参数
来源：http://www.share.bbcook.cn/Article/details/geoouqcal.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.tarul.cn/Article/details/giwusxcqr.sHtML

[R05] 参数默认值
来源：http://read.share.fktsv.cn/Article/details/gnqdtptvr.sHtML

name="${1:-default}"
来源：http://www.share.vehdjk.com/Article/details/ggkygbsco.sHtML

[R06] 判断命令是否存在
来源：http://www.share.epnwcf.com/Article/details/gerczxhqs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/gmyxwmlax.sHtML

[R07] if 判断文件
来源：http://wap.sjlbkw.cn/Article/details/gqlaoflno.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fktsv.cn/Article/details/gsbutwipf.sHtML

[R08] 数值比较
来源：http://blog.yfazqb.com/Article/details/gqaqthhqu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.sjlbkw.cn/Article/details/gvpndflrc.sHtML

[R09] 字符串比较
来源：http://wap.epnwcf.com/Article/details/gjclkalhr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.bbcook.cn/Article/details/geumbwvaj.sHtML

[R10] 正则匹配
来源：http://m.share.epnwcf.com/Article/details/gglrruspm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fktsv.cn/Article/details/gdbevcbqw.sHtML

[R11] case 多分支
来源：http://3g.sjlbkw.cn/Article/details/gxyqcunpx.sHtML

case "$1" in
来源：http://www.share.vehdjk.com/Article/details/gqhuyalmd.sHtML

start) echo "启动" ;;
来源：http://3g.epnwcf.com/Article/details/gydwauadz.sHtML

stop)  echo "停止" ;;
来源：http://baike.epnwcf.com/Article/details/griqyvtzk.sHtML

*)     echo "未知命令" ;;
来源：http://blog.sjlbkw.cn/Article/details/gyveccqye.sHtML

esac
来源：http://www.share.fktsv.cn/Article/details/gkquhqapn.sHtML

[R12] for 遍历文件
来源：http://wap.fktsv.cn/Article/details/giosopvvn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.tarul.cn/Article/details/glqdkijvx.sHtML

[R13] for 计数循环
来源：http://3g.yfazqb.com/Article/details/gbbkvattg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.epnwcf.com/Article/details/gucehdale.sHtML

[R14] C 风格 for
来源：http://3g.vehdjk.com/Article/details/gqktfwnvn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gvctfqlxf.sHtML

[R15] while 逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/goggorlin.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fktsv.cn/Article/details/gdpcsehoo.sHtML

[R16] until 等待条件
来源：http://www.m.share.tarul.cn/Article/details/gafktbqif.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.tarul.cn/Article/details/gaxlszrhu.sHtML

[R17] 数组定义与取值
来源：http://read.share.sjlbkw.cn/Article/details/gxbdaygzj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.vehdjk.com/Article/details/gbylthnwg.sHtML

[R18] 遍历数组
来源：http://mobile.vehdjk.com/Article/details/gfwrmxlxq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/ghflggurg.sHtML

[R19] 数组长度
来源：http://read.share.vehdjk.com/Article/details/gqtmdsvya.sHtML

echo "${#arr[@]}"
来源：http://read.share.fktsv.cn/Article/details/gpslxlwuj.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.vehdjk.com/Article/details/gzmhnabqe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.vehdjk.com/Article/details/gzcnlekwc.sHtML

[R21] 字符串长度
来源：http://baike.epnwcf.com/Article/details/ggejauxey.sHtML

echo "${#s}"
来源：http://www.share.fktsv.cn/Article/details/gtyddkgqg.sHtML

[R22] 截取子串
来源：http://baike.bbcook.cn/Article/details/gozojnphh.sHtML

echo "${s:0:5}"
来源：http://blog.yfazqb.com/Article/details/gmulgokbv.sHtML

[R23] 字符串替换
来源：http://www.m.share.yfazqb.com/Article/details/gapdmflqm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.epnwcf.com/Article/details/gssdqwrwx.sHtML

[R24] 大小写转换
来源：http://read.share.vehdjk.com/Article/details/gvmyadqzf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.tarul.cn/Article/details/gunbbmuuo.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.sjlbkw.cn/Article/details/gjnchdmrv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.bbcook.cn/Article/details/gmndphazv.sHtML

[R26] 命令替换
来源：http://read.share.sjlbkw.cn/Article/details/grmzaayms.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.epnwcf.com/Article/details/gobemefox.sHtML

[R27] 算术展开
来源：http://wap.yfazqb.com/Article/details/gnerubcvb.sHtML

echo $((1 + 2 * 3))
来源：http://baike.epnwcf.com/Article/details/gvnrxyyjh.sHtML

[R28] 浮点运算
来源：http://www.share.bbcook.cn/Article/details/gpatfysyq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrininyw.sHtML

[R29] 定义函数
来源：http://blog.bbcook.cn/Article/details/gfuyogouw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.tarul.cn/Article/details/ghiyutvwm.sHtML

[R30] 函数返回状态码
来源：http://blog.vehdjk.com/Article/details/gdyjchrfb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.tarul.cn/Article/details/gbdpamaxz.sHtML

[R31] 局部变量
来源：http://m.share.epnwcf.com/Article/details/gdvbjmrma.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.vehdjk.com/Article/details/gdtabeqaa.sHtML

[R32] 参数个数校验
来源：http://read.share.yfazqb.com/Article/details/gsjuxynzv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.tarul.cn/Article/details/gjazvnujr.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fktsv.cn/Article/details/gksuwvdhs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.vehdjk.com/Article/details/gytndyuqd.sHtML

[R34] 退出时清理
来源：http://www.blog.bbcook.cn/Article/details/gqywnjmwy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/gpbtobciv.sHtML

[R35] 后台执行并等待
来源：http://read.share.fktsv.cn/Article/details/gxsbtlles.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.sjlbkw.cn/Article/details/gqiugfvid.sHtML

[R36] 并发执行多个任务
来源：http://www.share.sjlbkw.cn/Article/details/gboipghzo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.tarul.cn/Article/details/gkbmwejhk.sHtML

[R37] 把输出赋给变量
来源：http://wap.epnwcf.com/Article/details/gtmthihyc.sHtML

files=$(ls -1)
来源：http://m.share.tarul.cn/Article/details/gjfrcwcbu.sHtML

[R38] 管道串联
来源：http://baike.tarul.cn/Article/details/gbfkypqvk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.epnwcf.com/Article/details/gpqixzkez.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.sjlbkw.cn/Article/details/gigkfgnmg.sHtML

cmd > out.log 2>&1
来源：http://www.blog.tarul.cn/Article/details/gninngxso.sHtML

[R40] 追加写日志
来源：http://blog.sjlbkw.cn/Article/details/gbkgymiax.sHtML

echo "log" >> out.log
来源：http://www.m.share.vehdjk.com/Article/details/gayudlswg.sHtML

[R41] 丢弃输出
来源：http://read.share.fktsv.cn/Article/details/gkraxnfpg.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.epnwcf.com/Article/details/gkconotkh.sHtML

[R42] 输入重定向
来源：http://mobile.tarul.cn/Article/details/gqwfmdcev.sHtML

wc -l < a.txt
来源：http://blog.epnwcf.com/Article/details/grpwkmkyu.sHtML

[R43] 按名字查找文件
来源：http://m.share.fktsv.cn/Article/details/gtswqppgm.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.bbcook.cn/Article/details/gyygtfyqc.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/gdhxtjgfj.sHtML

find . -mtime -7 -type f
来源：http://blog.fktsv.cn/Article/details/gvptqrznz.sHtML

[R45] 批量删除
来源：http://m.share.sjlbkw.cn/Article/details/ggkfvpvyo.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.tarul.cn/Article/details/gtvpeysku.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfvqynup.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.bbcook.cn/Article/details/gemlulplo.sHtML

[R47] sed 单行替换
来源：http://www.share.fktsv.cn/Article/details/guounsodw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gfvvmlvgj.sHtML

[R48] awk 取指定列
来源：http://m.share.vehdjk.com/Article/details/guswskqnq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gsszpleyd.sHtML

[R49] awk 带条件
来源：http://wap.fktsv.cn/Article/details/gthkbukom.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fktsv.cn/Article/details/ghlzjcvja.sHtML

[R50] awk 求和
来源：http://3g.bbcook.cn/Article/details/gfljdigip.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.tarul.cn/Article/details/ggsltjift.sHtML

[R51] 排序去重取前几
来源：http://baike.epnwcf.com/Article/details/gqjncdbqv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fktsv.cn/Article/details/gusgqvurc.sHtML

[R52] 统计行数
来源：http://www.blog.yfazqb.com/Article/details/ghhhlzsux.sHtML

wc -l a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gimrsagse.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.bbcook.cn/Article/details/giqtmfmop.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.bbcook.cn/Article/details/gmyuhvqzz.sHtML

[R54] 比较两个文件
来源：http://www.share.vehdjk.com/Article/details/gkkkextyc.sHtML

diff a.txt b.txt
来源：http://blog.sjlbkw.cn/Article/details/gpjcshyiw.sHtML

[R55] 压缩与解压
来源：http://wap.fktsv.cn/Article/details/gfubeaisx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.yfazqb.com/Article/details/gkcokvxmf.sHtML

[R56] 远程拷贝
来源：http://blog.vehdjk.com/Article/details/gxizecqxl.sHtML

scp file user@host:/path/
来源：http://m.share.vehdjk.com/Article/details/gpltnvmuv.sHtML

[R57] 远程执行命令
来源：http://www.blog.epnwcf.com/Article/details/gsrrrlfof.sHtML

ssh user@host 'uptime'
来源：http://baike.vehdjk.com/Article/details/ggxafzwpj.sHtML

[R58] 下载文件
来源：http://blog.vehdjk.com/Article/details/gaynqbhxj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.tarul.cn/Article/details/givhujidy.sHtML

[R59] 发 POST JSON
来源：http://read.share.fktsv.cn/Article/details/gglkukrer.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.tarul.cn/Article/details/gqzltzpjq.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/gtosuqtne.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fktsv.cn/Article/details/gnhgtkrwr.sHtML

[R61] 磁盘占用
来源：http://read.share.bbcook.cn/Article/details/ghccbmpfb.sHtML

df -h;  du -sh *
来源：http://mobile.sjlbkw.cn/Article/details/gmmxntrre.sHtML

[R62] 找最占空间的文件
来源：http://baike.tarul.cn/Article/details/gskpjrndg.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fktsv.cn/Article/details/ghffgdrmg.sHtML

[R63] 内存与进程
来源：http://mobile.vehdjk.com/Article/details/gpytbwcja.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.yfazqb.com/Article/details/gnmwhdfeo.sHtML

[R64] 结束进程
来源：http://blog.yfazqb.com/Article/details/gueijxsqu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggknwrzwg.sHtML

[R65] 查看端口占用
来源：http://blog.fktsv.cn/Article/details/glxulnrit.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.bbcook.cn/Article/details/gvqewabqt.sHtML

[R66] 定时任务
来源：http://blog.sjlbkw.cn/Article/details/guufrlwvv.sHtML

crontab -e;  crontab -l
来源：http://3g.yfazqb.com/Article/details/gtzewcuyw.sHtML

[R67] 生成随机十六进制串
来源：http://baike.tarul.cn/Article/details/gzfpnnwwt.sHtML

openssl rand -hex 16
来源：http://wap.bbcook.cn/Article/details/gzjkmsooh.sHtML

[R68] 计算文件校验值
来源：http://m.share.epnwcf.com/Article/details/gkqcfxvou.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.vehdjk.com/Article/details/ginesggtk.sHtML

[R69] 生成随机密码
来源：http://wap.vehdjk.com/Article/details/gwivwypfi.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.yfazqb.com/Article/details/gbxtrdlbr.sHtML

[R70] 时间戳与互转
来源：http://blog.yfazqb.com/Article/details/genjznljj.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.sjlbkw.cn/Article/details/gaotjuxum.sHtML

[R71] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/glqzskbnh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.sjlbkw.cn/Article/details/godyvvgbl.sHtML

[R72] 等待端口就绪
来源：http://wap.sjlbkw.cn/Article/details/guiackqnf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/gscjurfog.sHtML

[R73] 分割大日志
来源：http://www.m.share.yfazqb.com/Article/details/gzpgmmocr.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.epnwcf.com/Article/details/gqgwczvwq.sHtML

[R74] 批量重命名
来源：http://mobile.epnwcf.com/Article/details/gdxcfqvji.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.vehdjk.com/Article/details/gblxjvmpw.sHtML

[R75] 导出环境变量
来源：http://www.share.fktsv.cn/Article/details/gpegtxpzz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fktsv.cn/Article/details/grzelcgur.sHtML

[R76] 使用临时文件
来源：http://baike.vehdjk.com/Article/details/grxokrebk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/ghfexzkit.sHtML

[R77] 读取用户输入
来源：http://3g.tarul.cn/Article/details/gcpvtkahp.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.bbcook.cn/Article/details/gxhjnmceh.sHtML

[R78] 交互式菜单
来源：http://read.share.vehdjk.com/Article/details/gvlcqsgaz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fktsv.cn/Article/details/gifkhxupy.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvjewxvk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.bbcook.cn/Article/details/ghidbnfna.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.yfazqb.com/Article/details/gsgsmfckq.sHtML

time ./run.sh
来源：http://mobile.bbcook.cn/Article/details/gsklnaflr.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gpeaogmjy.sHtML

S. C / C++ 专题
来源：http://www.blog.vehdjk.com/Article/details/gkiztmycm.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gqmttxnol.sHtML

[S01] C：Hello World
来源：http://baike.tarul.cn/Article/details/ganncevoc.sHtML

#include <stdio.h>
来源：http://www.share.tarul.cn/Article/details/gyfdaxdpn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.tarul.cn/Article/details/gluytlwal.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/giaupcwdc.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fktsv.cn/Article/details/gbmbaetio.sHtML

[S03] C：读入整数
来源：http://mobile.yfazqb.com/Article/details/gytbrypzv.sHtML

int x; scanf("%d", &x);
来源：http://wap.vehdjk.com/Article/details/gwvsfejxx.sHtML

[S04] C：字符串复制
来源：http://read.share.sjlbkw.cn/Article/details/gjoanppjd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.yfazqb.com/Article/details/gnzbjniua.sHtML

[S05] C：字符串长度
来源：http://www.blog.fktsv.cn/Article/details/gzoegypym.sHtML

strlen(s)
来源：http://www.blog.vehdjk.com/Article/details/gwunyfsdm.sHtML

[S06] C：字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/glnidbssz.sHtML

strcmp(a, b) == 0
来源：http://blog.tarul.cn/Article/details/gbcjkhjur.sHtML

[S07] C：数组遍历求和
来源：http://blog.tarul.cn/Article/details/gwgssxxnm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fktsv.cn/Article/details/gauwjvihi.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.vehdjk.com/Article/details/gantnmvfq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.epnwcf.com/Article/details/gggeooblw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.epnwcf.com/Article/details/gxskwyuim.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.epnwcf.com/Article/details/gonjgbddu.sHtML

[S10] C：指针与解引用
来源：http://www.share.epnwcf.com/Article/details/gsahwxben.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.sjlbkw.cn/Article/details/ggxpfjsmo.sHtML

[S11] C：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gsbllzmer.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.tarul.cn/Article/details/gzqwimcgj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.bbcook.cn/Article/details/gvqaiutst.sHtML

fclose(f);
来源：http://blog.vehdjk.com/Article/details/gnrneenrd.sHtML

[S12] C：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gjzjwmfcg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.epnwcf.com/Article/details/gpfsngdgz.sHtML

[S13] C：宏定义
来源：http://www.blog.fktsv.cn/Article/details/ggnxyfhot.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.epnwcf.com/Article/details/gbwivxslw.sHtML

[S14] C：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gnvnnhpnv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.bbcook.cn/Article/details/gznbotjqf.sHtML

[S15] C：类型转换
来源：http://wap.epnwcf.com/Article/details/gbvrigygn.sHtML

(double) a / b
来源：http://www.share.vehdjk.com/Article/details/gmauebbcy.sHtML

[S16] C：位操作置位
来源：http://wap.bbcook.cn/Article/details/grhutyxzt.sHtML

x |= (1 << 3);
来源：http://www.blog.vehdjk.com/Article/details/gztkrbyhm.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gtnvuhdqg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.bbcook.cn/Article/details/gdrcaxbln.sHtML

[S18] C：命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/gxgfrvcgl.sHtML

int main(int argc, char **argv)
来源：http://www.share.tarul.cn/Article/details/gwqbhjrap.sHtML

[S19] C：快速排序
来源：http://wap.bbcook.cn/Article/details/gatxmsrwn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.vehdjk.com/Article/details/gdivnlili.sHtML

[S20] C：二分查找
来源：http://www.blog.sjlbkw.cn/Article/details/glptjzicy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gaqfdrbvd.sHtML

[S21] C：字符类别判断
来源：http://mobile.tarul.cn/Article/details/gvlbhtoej.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.yfazqb.com/Article/details/gqdsmdiqn.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.bbcook.cn/Article/details/gqinxocrr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.epnwcf.com/Article/details/gsyzrjpio.sHtML

[S23] C：随机数
来源：http://www.blog.epnwcf.com/Article/details/gjjjpxqrl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.epnwcf.com/Article/details/grgycfxmy.sHtML

[S24] C：获取本地时间
来源：http://blog.vehdjk.com/Article/details/gzwoblkjt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.yfazqb.com/Article/details/gmsxbesuw.sHtML

[S25] C：内存拷贝
来源：http://www.share.vehdjk.com/Article/details/ghflloeaa.sHtML

memcpy(dst, src, n);
来源：http://blog.sjlbkw.cn/Article/details/guvlnkxuc.sHtML

[S26] C：内存清零
来源：http://baike.yfazqb.com/Article/details/gxpquybuq.sHtML


<!-- 参考信息 -->