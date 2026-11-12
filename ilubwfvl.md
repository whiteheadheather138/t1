代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://zfz.nanxuanxn.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xee.kuanghao11.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://aih.snrcjt.cn

[Q15] 查询全部
来源：http://pcf.meibo888.top

SELECT * FROM users;
来源：http://ltv.bbcook.cn

[Q16] 查询指定列
来源：http://lkl.0kj1m.cn

SELECT id, name FROM users;
来源：http://tki.nanxinkj.top

[Q17] 条件查询
来源：http://tco.shanyushiyangtech.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pyr.yuxming.cn

[Q18] 模糊匹配
来源：http://qtx.ydzc1.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mxk.quarkkingdee.top

[Q19] 范围查询
来源：http://anm.svipenyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://psz.bbcook.cn

[Q20] IN 列表
来源：http://yhl.bbcook.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wgb.jyoumei.cn

[Q21] 空值判断
来源：http://oxj.ybcxt.top

SELECT * FROM users WHERE email IS NULL;
来源：http://aym.bjfxy.top

[Q22] 排序
来源：http://mwu.ydzc1.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gil.jinqigfzy.top

[Q23] 分页
来源：http://cre.zdbjq.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ivy.hysaishi.cn

[Q24] 去重
来源：http://atg.yonumen.top

SELECT DISTINCT city FROM users;
来源：http://jzt.fanxiaobao.xyz

[Q25] 只取前 N 条
来源：http://qdk.zdqjudy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eiq.9152youxi.cn

[Q26] 计数
来源：http://kuo.zdbjq.cn

SELECT COUNT(*) FROM users;
来源：http://wcm.gzhubu.top

[Q27] 条件计数
来源：http://iii.smart0.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://git.ppjwa.cn

[Q28] 求和与平均
来源：http://bdi.svipenyu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pvq.ywan-chungtsiang.top

[Q29] 最大最小值
来源：http://frq.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bjd.aibaodan.cn

[Q30] 分组统计
来源：http://mac.havefunace.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cus.jinghuilouyu.cn

[Q31] 分组后过滤
来源：http://clh.andypj.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rtt.yuxming.cn

[Q32] 分组拼接字符串
来源：http://lwb.zhengqikj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://csw.gzhubu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dkn.dashuyun.cn

[Q33] 多列分组
来源：http://tvk.tian-w.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gzb.jqgfzy.top

[Q34] 每组取第一条
来源：http://wsa.chenlongwang.top

SELECT * FROM (
来源：http://imh.pengpengdd.cyou

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uug.yj202588.top

) t WHERE rn = 1;
来源：http://qex.zhaomingkeji.xyz

[Q35] 内连接
来源：http://aim.daria6918.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eii.zhixingplan.top

[Q36] 左连接
来源：http://nkk.yuxming.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kvb.jyoumei.cn

[Q37] 右连接
来源：http://zds.uphjek.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://riq.uphjek.com

[Q38] 全外连接（PostgreSQL）
来源：http://roi.gaohongyu789.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://upm.xziqi.cn

[Q39] 自连接（查上下级）
来源：http://ukk.zhengqikj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ulb.havefunace.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eit.aizwys.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sbu.fktsv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wtr.gzhubu.top

[Q41] 多表连接
来源：http://rog.hywenlv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lkl.daria6918.cn

JOIN users u ON u.id = o.user_id
来源：http://hxe.hnxiangtu.top

JOIN products p ON p.id = o.product_id;
来源：http://zbv.shangyingyoupin.top

[Q42] 连接条件附加过滤
来源：http://wol.ppjwa.cn

SELECT u.name, o.amount FROM users u
来源：http://fll.gaohongyu789.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://whg.nwbrower.top

[Q43] 标量子查询
来源：http://fpk.quarkkingdee.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tkn.shuidangran.top

[Q44] IN 子查询
来源：http://mth.yuanzhike.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tok.pycfn.com

[Q45] EXISTS 判断存在
来源：http://qnn.zhijiandao.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xem.wangdashe.top

[Q46] NOT EXISTS 判断不存在
来源：http://qld.vqdsnc.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vqe.jinqigufen.top

[Q47] 与平均值比较
来源：http://bti.zhongyouzk.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://seb.fzhhl.top

[Q48] CTE 公用表表达式
来源：http://jcw.yueranfly.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pzi.kuanghao11.cn

SELECT * FROM t WHERE c > 5;
来源：http://elx.zhijiandao.cn

[Q49] 更新单行
来源：http://kwi.hesvh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ekf.jinyuanbaomall.cn

[Q50] 批量更新
来源：http://zxs.zdqjudy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fqj.vqdsnc.cn

[Q51] 用子查询更新
来源：http://dpa.ivvv.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zlv.0kj1m.cn

[Q52] 删除指定行
来源：http://cwe.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://ydb.jinghuilouyu.cn

[Q53] 按条件删除
来源：http://jxm.haohaochexian.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ydt.zhiwuduotai.top

[Q54] 清空表
来源：http://cxm.zdqjudy.top

TRUNCATE TABLE logs;
来源：http://lrn.jqgfzy.top

[Q55] 排名（并列占位）
来源：http://ifh.xuanzx.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fpw.yanxiufei.cn

[Q56] 密集排名（并列不占位）
来源：http://aoa.yuanzhike.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iqv.yonumen.top

[Q57] 行号
来源：http://laa.redwolf501.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nvw.yfazqb.com

[Q58] 累计求和
来源：http://zqi.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wuj.jlsjyb.cn

[Q59] 分组内累计
来源：http://hgt.cashguo.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lag.shangyingyoupin.top

[Q60] 取上一行 / 下一行
来源：http://yxm.bjfxy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lwi.zdbjq.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mub.yfazqb.com

[Q61] 移动平均
来源：http://hwt.zdbjq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yaf.vehdjk.com

[Q62] 分组占比
来源：http://wzs.jinqigfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xdl.shanyushiyangtech.top

[Q63] 开启事务
来源：http://jgl.jqgfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pog.nanxinkj.top

[Q64] 提交事务
来源：http://nss.fzhhl.top

COMMIT;
来源：http://axz.pengpengdd.cyou

[Q65] 回滚事务
来源：http://dun.vqdsnc.cn

ROLLBACK;
来源：http://hlu.yj20258888.top

[Q66] 行锁查询
来源：http://hlk.fanxiaobao.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://twb.ivvv.top

[Q67] 设置隔离级别
来源：http://box.xinyue.icu

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zwe.aibaodan.cn

[Q68] 保存点
来源：http://gbc.yuanzhike.top

SAVEPOINT sp1;
来源：http://vcs.ybcxt.top

ROLLBACK TO sp1;
来源：http://suk.hammf.cn

[Q69] 查看执行计划
来源：http://isa.shanyushiyangtech.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://miy.nwbrower.top

[Q70] 更新统计信息
来源：http://ejx.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://tbb.yongpay.top

[Q71] 查看建表语句
来源：http://nib.sxryk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gbb.bbcook.cn

[Q72] 查看索引
来源：http://olf.xylfe.cn

SHOW INDEX FROM users;
来源：http://vup.dashuyun.cn

[Q73] 查看表状态
来源：http://sps.tian-w.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ybq.fktsv.cn

[Q74] 强制使用索引
来源：http://uyy.fzhhl.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ofq.nanxuanxn.top

[Q75] 日期格式化
来源：http://idg.epnwcf.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zkw.hywenlv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qws.xylfe.cn

[Q76] 按天统计
来源：http://twx.jyoumei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wrb.meibo888.top

[Q77] 时间加减
来源：http://xgm.smart0.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rav.jinqigufen.top

[Q78] 当前时间
来源：http://yqf.yj20258.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ygt.yueranfly.top

[Q79] 字符串拼接
来源：http://fut.hcnkem.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tvt.fehbvm.com

[Q80] 字符串截取
来源：http://dwh.tian-w.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hlk.yueranfly.top

[Q81] 字符串替换
来源：http://yyt.zhiwuduotai.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bki.cqqwz.cn

[Q82] 字符长度与字节长度
来源：http://hxj.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hlp.chenlongwang.top

[Q83] 大小写转换
来源：http://bjv.tianlin.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kjk.yonumen.top

[Q84] 去除首尾空格
来源：http://szx.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://clg.yongpay.top

[Q85] 数值取整
来源：http://llm.jlsjyb.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zak.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://fqc.hongshengwenyu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qxq.svipenyu.cn

[Q87] JSON 字段做条件
来源：http://nyc.wangshuangyany.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://irx.cucudq.cn

[Q88] 行转列（条件聚合）
来源：http://fee.zhiwuduotai.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xng.cashguo.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://irc.ppjwa.cn

[Q89] 判断表是否存在
来源：http://chb.c1oappe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zwj.jyoumei.cn

[Q90] 生成序号列
来源：http://dus.havefunace.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zbn.epnwcf.com

================================================================================
来源：http://cab.c1oappe.top

R. Bash 专题
来源：http://ssy.svipenyu.cn

================================================================================
来源：http://djk.svipenyu.cn

[R01] shebang 与严格模式
来源：http://shs.zhixingplan.top

#!/usr/bin/env bash
来源：http://rla.yongpay.top

set -euo pipefail
来源：http://hxg.daria6918.cn

[R02] 变量赋值与使用
来源：http://qht.cashguo.top

name="Tom"; echo "$name"
来源：http://tzr.shangyingyoupin.top

[R03] 只读变量
来源：http://cil.hnqzz.top

readonly PI=3.14
来源：http://bmf.tianlin.xyz

[R04] 位置参数
来源：http://zov.sweek.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dxh.hesvh.cn

[R05] 参数默认值
来源：http://agy.daxiang520.top

name="${1:-default}"
来源：http://cww.vehdjk.com

[R06] 判断命令是否存在
来源：http://uwl.hfpthk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cno.tarul.cn

[R07] if 判断文件
来源：http://kbx.sufxvd.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fel.ivvv.top

[R08] 数值比较
来源：http://yph.yj20258888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ggu.jinghuilouyu.cn

[R09] 字符串比较
来源：http://iov.yfazqb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wkh.nwbrower.top

[R10] 正则匹配
来源：http://cfp.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ugv.tianlin.xyz

[R11] case 多分支
来源：http://ftw.svipenyu.cn

case "$1" in
来源：http://fwk.ybcxt.top

start) echo "启动" ;;
来源：http://ryr.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://vkb.zhijiandao.cn

*)     echo "未知命令" ;;
来源：http://ezo.ctjpmb.com

esac
来源：http://lac.mhx1999.top

[R12] for 遍历文件
来源：http://nof.tianlin.xyz

for f in *.txt; do echo "$f"; done
来源：http://qwm.gzhubu.top

[R13] for 计数循环
来源：http://yor.zycfv.cn

for i in {1..10}; do echo "$i"; done
来源：http://izo.redwolf501.top

[R14] C 风格 for
来源：http://mdo.havefunace.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rse.sufxvd.cn

[R15] while 逐行读文件
来源：http://nlj.cucudq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tiq.sufxvd.cn

[R16] until 等待条件
来源：http://iwn.pycfn.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hsg.shzxlz.cn

[R17] 数组定义与取值
来源：http://yad.zhixingplan.top

arr=(a b c); echo "${arr[0]}"
来源：http://nel.hesvh.cn

[R18] 遍历数组
来源：http://dke.chenzaomai.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dkg.hysaishi.cn

[R19] 数组长度
来源：http://biq.zhongyouzk.top

echo "${#arr[@]}"
来源：http://lve.52xcode.cn

[R20] 关联数组（字典）
来源：http://zoy.cdnleiting.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jtl.fengsongda.top

[R21] 字符串长度
来源：http://usc.redwolf501.top

echo "${#s}"
来源：http://dlf.yj202588.top

[R22] 截取子串
来源：http://whw.sysykeji.top

echo "${s:0:5}"
来源：http://bvo.tianlin.xyz

[R23] 字符串替换
来源：http://rkc.chenzaomai.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xas.jiagoushi.top

[R24] 大小写转换
来源：http://byr.chenjidiqi.icu

echo "${s^^}"; echo "${s,,}"
来源：http://lef.xinyue.icu

[R25] 去后缀 / 去前缀
来源：http://ixd.gaohongyu789.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fdb.smart0.xyz

[R26] 命令替换
来源：http://byg.iojbl.cn

now=$(date +%F); echo "$now"
来源：http://dkr.yuxming.cn

[R27] 算术展开
来源：http://tbo.hywenlv.cn

echo $((1 + 2 * 3))
来源：http://oft.ivvv.top

[R28] 浮点运算
来源：http://bqt.jinyuanbaomall.cn

echo "scale=2; 10/3" | bc
来源：http://jhf.ppjwa.cn

[R29] 定义函数
来源：http://ndm.zdqjudy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://aqg.jyoumei.cn

[R30] 函数返回状态码
来源：http://cjx.zdqjudy.top

f() { return 0; }; f || echo "失败了"
来源：http://rhx.jinqigfzy.top

[R31] 局部变量
来源：http://hgh.pycfn.com

f() { local x=1; echo "$x"; }
来源：http://ajx.jiagoushi.top

[R32] 参数个数校验
来源：http://wvn.guowangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://plj.nanxinkj.top

[R33] 捕获错误并提示行号
来源：http://ekv.dianchejie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lkb.quarkkingdee.top

[R34] 退出时清理
来源：http://sck.hnxiangtu.top

trap 'rm -f "$tmp"' EXIT
来源：http://ves.chenlongwang.top

[R35] 后台执行并等待
来源：http://hlv.vqdsnc.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mzn.shangyingyoupin.top

[R36] 并发执行多个任务
来源：http://pet.sweek.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tbj.0kj1m.cn

[R37] 把输出赋给变量
来源：http://vkb.iojbl.cn

files=$(ls -1)
来源：http://lkt.gogol.net.cn

[R38] 管道串联
来源：http://omq.0kj1m.cn

cat a.txt | grep -i error | wc -l
来源：http://uvr.yuanzhike.top

[R39] 重定向标准输出与错误
来源：http://gmv.jianghu66.top

cmd > out.log 2>&1
来源：http://cwr.316326.xyz

[R40] 追加写日志
来源：http://uts.zhixingplan.top

echo "log" >> out.log
来源：http://vbp.9152youxi.cn

[R41] 丢弃输出
来源：http://xtl.kuanghao11.cn

cmd >/dev/null 2>&1
来源：http://iqs.yj202588.top

[R42] 输入重定向
来源：http://ooy.gogol.net.cn

wc -l < a.txt
来源：http://bwl.pycfn.com

[R43] 按名字查找文件
来源：http://fde.yueranfly.top

find . -name "*.log" -type f
来源：http://hdg.shuidangran.top

[R44] 按修改时间查找
来源：http://owu.chenjidiqi.icu

find . -mtime -7 -type f
来源：http://ixc.yfazqb.com

[R45] 批量删除
来源：http://ysz.hfpthk.cn

find . -name "*.tmp" -delete
来源：http://vnc.haohaochexian.top

[R46] 递归替换文件内容
来源：http://pam.hysaishi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fwj.meibo888.top

[R47] sed 单行替换
来源：http://zef.yj202588.top

sed -i 's/foo/bar/g' a.txt
来源：http://cep.sjlbkw.cn

[R48] awk 取指定列
来源：http://zqe.xingfuxueyuan.xyz

awk '{print $1, $3}' a.txt
来源：http://wsb.redwolf501.top

[R49] awk 带条件
来源：http://lll.hammf.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aqb.wangshuangyany.cn

[R50] awk 求和
来源：http://trr.sufxvd.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bkp.nanxuanxn.top

[R51] 排序去重取前几
来源：http://zyg.tanke756.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qif.feifeiyinyue.top

[R52] 统计行数
来源：http://wxl.hnqzz.top

wc -l a.txt
来源：http://nat.ydjk.org.cn

[R53] 查看文件头与实时尾
来源：http://vwt.haohaochexian.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wfm.iojbl.cn

[R54] 比较两个文件
来源：http://xtd.chenzaomai.com

diff a.txt b.txt
来源：http://mcl.chenjidiqi.icu

[R55] 压缩与解压
来源：http://qmz.zycfv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mhd.svipenyu.cn

[R56] 远程拷贝
来源：http://xbl.gotoacloud.top

scp file user@host:/path/
来源：http://axo.zdbjq.cn

[R57] 远程执行命令
来源：http://dby.guannengcc.top

ssh user@host 'uptime'
来源：http://ndx.havefunace.top

[R58] 下载文件
来源：http://pny.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hyc.snrcjt.cn

[R59] 发 POST JSON
来源：http://ccq.gaohongyu789.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bhy.hesvh.cn

[R60] 只看 HTTP 状态码
来源：http://rte.aizwys.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cdw.hnqzz.top

[R61] 磁盘占用
来源：http://qff.jinqigufen.top

df -h;  du -sh *
来源：http://lhe.ywan-chungtsiang.top

[R62] 找最占空间的文件
来源：http://hbl.ybcxt.top

du -ah . | sort -rh | head -10
来源：http://woq.fanxiaobao.xyz

[R63] 内存与进程
来源：http://ylk.316326.xyz


<!-- 参考信息 -->