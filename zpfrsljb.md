代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lcu.yfazqb.com

[Q11] 一次插入多行
来源：http://pgh.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pqi.cheryme.top

[Q12] 插入后取自增 ID
来源：http://sqd.svipenyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vqk.guowangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sdg.0kj1m.cn

[Q13] 忽略重复插入
来源：http://kkt.tanke756.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tzp.jinyuanbaomall.cn

[Q14] 存在则更新（upsert）
来源：http://oke.nwbrower.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sja.zdqjudy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://beo.tian-w.cn

[Q15] 查询全部
来源：http://owa.meibo888.top

SELECT * FROM users;
来源：http://rhz.havefunace.top

[Q16] 查询指定列
来源：http://wke.ctjpmb.com

SELECT id, name FROM users;
来源：http://pns.316326.xyz

[Q17] 条件查询
来源：http://kou.316326.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uqb.jqgfzy.top

[Q18] 模糊匹配
来源：http://jtr.ydjk.org.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nux.sweek.top

[Q19] 范围查询
来源：http://pvn.nanxuanxn.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xyr.ehwqpu.com

[Q20] IN 列表
来源：http://gzb.mhx1999.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://alb.zhengqikj.top

[Q21] 空值判断
来源：http://mbs.uphjek.com

SELECT * FROM users WHERE email IS NULL;
来源：http://bwu.tianlin.xyz

[Q22] 排序
来源：http://pco.ehwqpu.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gqk.hesvh.cn

[Q23] 分页
来源：http://gcz.ydjk.org.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://frk.zhiwuduotai.top

[Q24] 去重
来源：http://esf.nwbrower.top

SELECT DISTINCT city FROM users;
来源：http://jlf.bjfxy.top

[Q25] 只取前 N 条
来源：http://mdn.vqdsnc.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cyz.yj20258888.top

[Q26] 计数
来源：http://phd.smart0.xyz

SELECT COUNT(*) FROM users;
来源：http://eya.yanxiufei.cn

[Q27] 条件计数
来源：http://tdf.jiagoushi.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qbm.jqgfzy.top

[Q28] 求和与平均
来源：http://dod.ppjwa.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bmo.xziqi.cn

[Q29] 最大最小值
来源：http://got.jqgfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://sto.hfpthk.cn

[Q30] 分组统计
来源：http://ioa.sjlbkw.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rdj.yfazqb.com

[Q31] 分组后过滤
来源：http://zxy.hesvh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://may.pengpengdd.cyou

[Q32] 分组拼接字符串
来源：http://ysb.ydjk.org.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nwa.daxiang520.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://thl.bjfxy.top

[Q33] 多列分组
来源：http://dju.tarul.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yvc.shanyushiyangtech.top

[Q34] 每组取第一条
来源：http://npt.vqdsnc.cn

SELECT * FROM (
来源：http://zmn.gogol.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tfx.birdmap.top

) t WHERE rn = 1;
来源：http://hby.kuanghao11.cn

[Q35] 内连接
来源：http://jqy.jinqigfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ydl.yfazqb.com

[Q36] 左连接
来源：http://zqx.quarkkingdee.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xie.ctjpmb.com

[Q37] 右连接
来源：http://rxd.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://key.zhoulong.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://vfp.zhixingplan.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uvp.epnwcf.com

[Q39] 自连接（查上下级）
来源：http://xgl.nwbrower.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zze.jinyuanbaomall.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://son.chenjidiqi.icu

[Q40] 交叉连接（笛卡尔积）
来源：http://fpo.ybcxt.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://utc.snrcjt.cn

[Q41] 多表连接
来源：http://iug.ywan-chungtsiang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://yzy.shanyushiyangkeji.top

JOIN users u ON u.id = o.user_id
来源：http://aaq.meibo888.top

JOIN products p ON p.id = o.product_id;
来源：http://qco.hcnkem.com

[Q42] 连接条件附加过滤
来源：http://qno.cheryme.top

SELECT u.name, o.amount FROM users u
来源：http://kkc.havefunace.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yiz.ydjk.org.cn

[Q43] 标量子查询
来源：http://prs.jqgfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://apu.hongshengwenyu.top

[Q44] IN 子查询
来源：http://uky.hcnkem.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wth.jqgfzy.top

[Q45] EXISTS 判断存在
来源：http://ktc.shanyushiyangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://evd.hammf.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qha.feifeiyinyue.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fzr.birdmap.top

[Q47] 与平均值比较
来源：http://kjj.redwolf501.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://edj.haohaochexian.top

[Q48] CTE 公用表表达式
来源：http://afx.chenlongwang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cjc.xziqi.cn

SELECT * FROM t WHERE c > 5;
来源：http://yey.sufxvd.cn

[Q49] 更新单行
来源：http://lqt.pengpengdd.cyou

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vxj.meibo888.top

[Q50] 批量更新
来源：http://xct.gaohongyu789.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xel.0kj1m.cn

[Q51] 用子查询更新
来源：http://gpl.xziqi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://frr.svipenyu.cn

[Q52] 删除指定行
来源：http://xgo.jinqigfzy.top

DELETE FROM users WHERE id = 10;
来源：http://pza.fzhhl.top

[Q53] 按条件删除
来源：http://hig.yangfankeji.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nzm.nanxinkj.top

[Q54] 清空表
来源：http://gmx.kuanghao11.cn

TRUNCATE TABLE logs;
来源：http://mwp.zhiwuduotai.top

[Q55] 排名（并列占位）
来源：http://son.hongshengwenyu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oan.zdbjq.cn

[Q56] 密集排名（并列不占位）
来源：http://wwq.smart0.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://brk.ivvv.top

[Q57] 行号
来源：http://eim.jqgufenzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://muj.nanxinkj.top

[Q58] 累计求和
来源：http://gqo.yfazqb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jky.jianghu66.top

[Q59] 分组内累计
来源：http://vba.chenlongwang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://txu.jqgufenzy.top

[Q60] 取上一行 / 下一行
来源：http://rbf.sweek.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gfb.yanxiufei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oik.guannengcc.top

[Q61] 移动平均
来源：http://ljo.yongpay.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mlp.shangyingyoupin.top

[Q62] 分组占比
来源：http://zdj.zhaomingkeji.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pcr.yj20258888.top

[Q63] 开启事务
来源：http://nfx.fengsongda.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dlu.fehbvm.com

[Q64] 提交事务
来源：http://ipm.cqqwz.cn

COMMIT;
来源：http://wpe.wangshuangyany.cn

[Q65] 回滚事务
来源：http://zkw.ydjk.org.cn

ROLLBACK;
来源：http://xwb.gzhubu.top

[Q66] 行锁查询
来源：http://ajh.xuetiantiany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dip.hysaishi.cn

[Q67] 设置隔离级别
来源：http://dox.zhongyouzk.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mer.chenzaomai.com

[Q68] 保存点
来源：http://doj.shanyushiyangtech.top

SAVEPOINT sp1;
来源：http://dzd.vehdjk.com

ROLLBACK TO sp1;
来源：http://ovv.snrcjt.cn

[Q69] 查看执行计划
来源：http://dls.jinqigufen.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vvg.tian-w.cn

[Q70] 更新统计信息
来源：http://osy.yanxiufei.cn

ANALYZE TABLE users;
来源：http://hzb.yvedp.cn

[Q71] 查看建表语句
来源：http://gks.kuanghao11.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://thx.chenlongwang.top

[Q72] 查看索引
来源：http://kzc.bjfxy.top

SHOW INDEX FROM users;
来源：http://npm.0kj1m.cn

[Q73] 查看表状态
来源：http://jbh.shanyushiyangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ktc.xylfe.cn

[Q74] 强制使用索引
来源：http://zlz.hywenlv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bvr.cheryme.top

[Q75] 日期格式化
来源：http://tkh.yanxiufei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jbv.gotoacloud.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wpd.ppjwa.cn

[Q76] 按天统计
来源：http://guw.mhx1999.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kpp.sjlbkw.cn

[Q77] 时间加减
来源：http://ona.fehbvm.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ppt.chenzaomai.com

[Q78] 当前时间
来源：http://iez.0kj1m.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://krv.yfazqb.com

[Q79] 字符串拼接
来源：http://xyj.yfazqb.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://psm.zdqjudy.top

[Q80] 字符串截取
来源：http://wco.fktsv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fna.gzhubu.top

[Q81] 字符串替换
来源：http://etb.snrcjt.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vzn.bjfxy.top

[Q82] 字符长度与字节长度
来源：http://bno.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ulh.jinqigufen.top

[Q83] 大小写转换
来源：http://tqy.hysaishi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hqn.gogol.net.cn

[Q84] 去除首尾空格
来源：http://hxd.smart0.xyz

SELECT TRIM(name) FROM users;
来源：http://zur.ehwqpu.com

[Q85] 数值取整
来源：http://rsi.tarul.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dqv.gaohongyu789.top

[Q86] 读取 JSON 字段
来源：http://qli.aibaodan.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jen.xingfuxueyuan.xyz

[Q87] JSON 字段做条件
来源：http://hpr.ydjk.org.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cax.hysaishi.cn

[Q88] 行转列（条件聚合）
来源：http://ehb.jinyuanbaomall.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xly.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eik.yueranfly.top

[Q89] 判断表是否存在
来源：http://lhe.zhijiandao.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ekr.redwolf501.top

[Q90] 生成序号列
来源：http://jzc.yfazqb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uzh.chenzaomai.com

================================================================================
来源：http://aiu.shanyushiyangtech.top

R. Bash 专题
来源：http://dhs.jqgufenzy.top

================================================================================
来源：http://cap.zhiwuduotai.top

[R01] shebang 与严格模式
来源：http://oar.guannengcc.top

#!/usr/bin/env bash
来源：http://roi.yj20258.top

set -euo pipefail
来源：http://gif.ywan-chungtsiang.top

[R02] 变量赋值与使用
来源：http://ieh.dashuyun.cn

name="Tom"; echo "$name"
来源：http://xod.yj202588.top

[R03] 只读变量
来源：http://gqd.jqgufenzy.top

readonly PI=3.14
来源：http://bfl.bjfxy.top

[R04] 位置参数
来源：http://gtm.gotoacloud.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gbj.birdmap.top

[R05] 参数默认值
来源：http://lda.yanxiufei.cn

name="${1:-default}"
来源：http://krm.jqgfzy.top

[R06] 判断命令是否存在
来源：http://sds.tian-w.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oxr.yuxming.cn

[R07] if 判断文件
来源：http://tid.yueranfly.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xgm.daxiang520.top

[R08] 数值比较
来源：http://vaz.zhaomingkeji.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://bjr.zhongyouzk.top

[R09] 字符串比较
来源：http://yui.yanxiufei.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mnq.ydzc1.top

[R10] 正则匹配
来源：http://rer.yonumen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gbr.tarul.cn

[R11] case 多分支
来源：http://hlc.xinyue.icu

case "$1" in
来源：http://aff.xziqi.cn

start) echo "启动" ;;
来源：http://sfa.hnxiangtu.top

stop)  echo "停止" ;;
来源：http://oqo.sxryk.cn

*)     echo "未知命令" ;;
来源：http://ddf.yueranfly.top

esac
来源：http://tmc.zhongyouzk.top

[R12] for 遍历文件
来源：http://hcc.cashguo.top

for f in *.txt; do echo "$f"; done
来源：http://pxl.tanke756.top

[R13] for 计数循环
来源：http://nwg.havefunace.top

for i in {1..10}; do echo "$i"; done
来源：http://pta.zhixingplan.top

[R14] C 风格 for
来源：http://asy.jqgfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ktg.hnxiangtu.top

[R15] while 逐行读文件
来源：http://dry.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wgm.zhengqikj.top

[R16] until 等待条件
来源：http://yhu.cdnleiting.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cfw.jinghuilouyu.cn

[R17] 数组定义与取值
来源：http://kur.ctjpmb.com

arr=(a b c); echo "${arr[0]}"
来源：http://vga.zhoulong.xyz

[R18] 遍历数组
来源：http://smm.kuanghao11.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qtv.hysaishi.cn

[R19] 数组长度
来源：http://fko.52xcode.cn

echo "${#arr[@]}"
来源：http://tnn.shzxlz.cn

[R20] 关联数组（字典）
来源：http://cnb.jiagoushi.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zyk.nanxinkj.top

[R21] 字符串长度
来源：http://mha.zhijiandao.cn

echo "${#s}"
来源：http://zrd.zdbjq.cn

[R22] 截取子串
来源：http://fxq.hnxiangtu.top

echo "${s:0:5}"
来源：http://pns.zhixingplan.top

[R23] 字符串替换
来源：http://zwr.fktsv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ghs.snrcjt.cn

[R24] 大小写转换
来源：http://pwy.zhongyouzk.top

echo "${s^^}"; echo "${s,,}"
来源：http://wjo.epnwcf.com

[R25] 去后缀 / 去前缀
来源：http://zij.zhaomingkeji.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://cxm.daria6918.cn

[R26] 命令替换
来源：http://qfl.dianchejie.cn

now=$(date +%F); echo "$now"
来源：http://osa.hfpthk.cn

[R27] 算术展开
来源：http://dig.mhx1999.top

echo $((1 + 2 * 3))
来源：http://jye.gogol.net.cn

[R28] 浮点运算
来源：http://usz.yangfankeji.com

echo "scale=2; 10/3" | bc
来源：http://kyz.xziqi.cn

[R29] 定义函数
来源：http://dam.fengsongda.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://glf.hywenlv.cn

[R30] 函数返回状态码
来源：http://onb.c1oappe.top

f() { return 0; }; f || echo "失败了"
来源：http://idn.fengsongda.top

[R31] 局部变量
来源：http://fqj.sysykeji.top

f() { local x=1; echo "$x"; }
来源：http://wbo.daxiang520.top

[R32] 参数个数校验
来源：http://jop.yfazqb.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://met.dianchejie.cn

[R33] 捕获错误并提示行号
来源：http://xek.zhoulong.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ego.fengsongda.top

[R34] 退出时清理
来源：http://vto.hesvh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zcd.jiagoushi.top

[R35] 后台执行并等待
来源：http://snx.sjlbkw.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://utz.gotoacloud.top

[R36] 并发执行多个任务
来源：http://spq.jiagoushi.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fjg.jlsjyb.cn

[R37] 把输出赋给变量
来源：http://tvo.zhijiandao.cn

files=$(ls -1)
来源：http://les.zhongyouzk.top

[R38] 管道串联
来源：http://kzh.shanyushiyangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://npv.guannengcc.top

[R39] 重定向标准输出与错误
来源：http://ees.xylfe.cn

cmd > out.log 2>&1
来源：http://ezg.pycfn.com

[R40] 追加写日志
来源：http://qly.aizwys.cn

echo "log" >> out.log
来源：http://zyp.zhengqikj.top

[R41] 丢弃输出
来源：http://bzx.sysykeji.top

cmd >/dev/null 2>&1
来源：http://onu.zhaomingkeji.xyz

[R42] 输入重定向
来源：http://dgt.pengpengdd.cyou

wc -l < a.txt
来源：http://suy.ivvv.top

[R43] 按名字查找文件
来源：http://gma.mhx1999.top

find . -name "*.log" -type f
来源：http://fmw.hammf.cn

[R44] 按修改时间查找
来源：http://nqy.hywenlv.cn

find . -mtime -7 -type f
来源：http://miz.tanke756.top

[R45] 批量删除
来源：http://bfa.hcnkem.com

find . -name "*.tmp" -delete
来源：http://ezm.chenlongwang.top

[R46] 递归替换文件内容
来源：http://puj.yj202588.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xiu.cashguo.top

[R47] sed 单行替换
来源：http://xay.hnqzz.top

sed -i 's/foo/bar/g' a.txt
来源：http://pfi.fengsongda.top

[R48] awk 取指定列
来源：http://dgu.nanxuanxn.top

awk '{print $1, $3}' a.txt
来源：http://xtf.jinqigufen.top

[R49] awk 带条件
来源：http://nur.hnqzz.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zlf.52xcode.cn

[R50] awk 求和
来源：http://obc.zhixingplan.top

awk '{s += $2} END {print s}' a.txt
来源：http://thh.hnqzz.top

[R51] 排序去重取前几
来源：http://chd.c1oappe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://eak.hysaishi.cn

[R52] 统计行数
来源：http://sbz.wangdashe.top

wc -l a.txt
来源：http://oop.shuidangran.top

[R53] 查看文件头与实时尾
来源：http://pau.uphjek.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kkw.jianghu66.top

[R54] 比较两个文件
来源：http://fsl.jinghuilouyu.cn

diff a.txt b.txt
来源：http://flk.zdbjq.cn

[R55] 压缩与解压
来源：http://nzf.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iwg.hammf.cn

[R56] 远程拷贝
来源：http://gsz.sjlbkw.cn

scp file user@host:/path/
来源：http://rkx.xylfe.cn

[R57] 远程执行命令
来源：http://loa.hnxiangtu.top

ssh user@host 'uptime'
来源：http://wea.jiagoushi.top

[R58] 下载文件
来源：http://njm.52xcode.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://azr.ppjwa.cn

[R59] 发 POST JSON
来源：http://mlk.aizwys.cn


<!-- 参考信息 -->