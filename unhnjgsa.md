代发 wailian999

);
来源：http://kmu.xylfe.cn

[Q03] 增加列
来源：http://zrg.jyoumei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://evs.gaohongyu789.top

[Q04] 修改列类型
来源：http://hud.yuanzhike.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ozn.ybcxt.top

[Q05] 重命名列
来源：http://cuj.zhoulong.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://trd.xuanzx.com

[Q06] 删除列
来源：http://fyj.ehwqpu.com

ALTER TABLE users DROP COLUMN age;
来源：http://kpq.fengsongda.top

[Q07] 删除表
来源：http://ycf.jinyuanbaomall.cn

DROP TABLE IF EXISTS orders;
来源：http://deb.hammf.cn

[Q08] 创建普通索引
来源：http://rmt.pycfn.com

CREATE INDEX idx_users_email ON users(email);
来源：http://oew.nanxuanxn.top

[Q09] 创建唯一索引
来源：http://odd.nanxinkj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dgr.bjfxy.top

[Q10] 插入单行
来源：http://ftc.smart0.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jkh.smart0.xyz

[Q11] 一次插入多行
来源：http://wnl.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pbx.zdbjq.cn

[Q12] 插入后取自增 ID
来源：http://cnc.sweek.top

INSERT INTO users (name) VALUES ('C');
来源：http://eqa.jianghu66.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ecj.ybcxt.top

[Q13] 忽略重复插入
来源：http://uqp.dianchejie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mwd.jinghuilouyu.cn

[Q14] 存在则更新（upsert）
来源：http://atb.jianghu66.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zgm.dianchejie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dzq.birdmap.top

[Q15] 查询全部
来源：http://idp.sxryk.cn

SELECT * FROM users;
来源：http://qbm.dashuyun.cn

[Q16] 查询指定列
来源：http://gzz.epnwcf.com

SELECT id, name FROM users;
来源：http://kbq.yvedp.cn

[Q17] 条件查询
来源：http://jhv.wangdashe.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bnd.mhx1999.top

[Q18] 模糊匹配
来源：http://smw.yj202588.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sgh.daxiang520.top

[Q19] 范围查询
来源：http://nty.gogol.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xaf.ehwqpu.com

[Q20] IN 列表
来源：http://yiy.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xkz.gaohongyu789.top

[Q21] 空值判断
来源：http://shx.9152youxi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mxt.zycfv.cn

[Q22] 排序
来源：http://zui.uphjek.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vjg.iojbl.cn

[Q23] 分页
来源：http://ngi.dashuyun.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zpp.shuidangran.top

[Q24] 去重
来源：http://mgh.wangdashe.top

SELECT DISTINCT city FROM users;
来源：http://vtu.cashguo.top

[Q25] 只取前 N 条
来源：http://yep.sysykeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://afj.fktsv.cn

[Q26] 计数
来源：http://xmf.nanxuanxn.top

SELECT COUNT(*) FROM users;
来源：http://bxg.hnxiangtu.top

[Q27] 条件计数
来源：http://lbk.c1oappe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hxe.tanke756.top

[Q28] 求和与平均
来源：http://ado.tianlin.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yvm.hammf.cn

[Q29] 最大最小值
来源：http://ork.daxiang520.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://huz.kuanghao11.cn

[Q30] 分组统计
来源：http://jyr.uphjek.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vtj.mhx1999.top

[Q31] 分组后过滤
来源：http://ikz.hongshengwenyu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yfh.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://emu.andypj.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ras.xinyue.icu

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wqe.cdnleiting.top

[Q33] 多列分组
来源：http://dhm.guowangkeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dbx.yueranfly.top

[Q34] 每组取第一条
来源：http://bmx.sysykeji.top

SELECT * FROM (
来源：http://snr.yvedp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://brm.shuidangran.top

) t WHERE rn = 1;
来源：http://jen.chenlongwang.top

[Q35] 内连接
来源：http://mua.wangshuangyany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://smi.feifeiyinyue.top

[Q36] 左连接
来源：http://xjo.feifeiyinyue.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uas.birdmap.top

[Q37] 右连接
来源：http://qmj.shangyingyoupin.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qqs.kuanghao11.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vhg.gzhubu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lzb.daxiang520.top

[Q39] 自连接（查上下级）
来源：http://wrd.ehwqpu.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://gfy.zycfv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://opr.haohaochexian.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hfo.nanxinkj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zcx.guannengcc.top

[Q41] 多表连接
来源：http://mtp.quarkkingdee.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://shr.bjfxy.top

JOIN users u ON u.id = o.user_id
来源：http://yay.gaohongyu789.top

JOIN products p ON p.id = o.product_id;
来源：http://rif.vqdsnc.cn

[Q42] 连接条件附加过滤
来源：http://rrx.yj20258888.top

SELECT u.name, o.amount FROM users u
来源：http://joi.zdbjq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://byp.nanxuanxn.top

[Q43] 标量子查询
来源：http://rtp.fehbvm.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kaq.ppjwa.cn

[Q44] IN 子查询
来源：http://wwo.zhongyouzk.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gsd.redwolf501.top

[Q45] EXISTS 判断存在
来源：http://elu.daria6918.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qsw.zhiwuduotai.top

[Q46] NOT EXISTS 判断不存在
来源：http://vpp.xuetiantiany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rfw.mhx1999.top

[Q47] 与平均值比较
来源：http://cui.hammf.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xal.yangfankeji.com

[Q48] CTE 公用表表达式
来源：http://mcf.epnwcf.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mwn.yuxming.cn

SELECT * FROM t WHERE c > 5;
来源：http://qwz.birdmap.top

[Q49] 更新单行
来源：http://byu.yj20258888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gyt.snrcjt.cn

[Q50] 批量更新
来源：http://drg.shanyushiyangtech.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://klg.pycfn.com

[Q51] 用子查询更新
来源：http://fce.dianchejie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pka.yanxiufei.cn

[Q52] 删除指定行
来源：http://nuj.havefunace.top

DELETE FROM users WHERE id = 10;
来源：http://fka.zhixingplan.top

[Q53] 按条件删除
来源：http://ooh.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mdz.pengpengdd.cyou

[Q54] 清空表
来源：http://eov.316326.xyz

TRUNCATE TABLE logs;
来源：http://mvh.jiagoushi.top

[Q55] 排名（并列占位）
来源：http://bes.316326.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://snz.shzxlz.cn

[Q56] 密集排名（并列不占位）
来源：http://tay.chenzaomai.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xal.meibo888.top

[Q57] 行号
来源：http://uxv.yongpay.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cgu.zhixingplan.top

[Q58] 累计求和
来源：http://jaz.ctjpmb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jqh.zhengqikj.top

[Q59] 分组内累计
来源：http://orr.wangdashe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rli.hnqzz.top

[Q60] 取上一行 / 下一行
来源：http://dqw.fengsongda.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ksu.jinqigufen.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://csc.xuetiantiany.cn

[Q61] 移动平均
来源：http://ahm.zhiwuduotai.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zzj.jianghu66.top

[Q62] 分组占比
来源：http://rwn.vehdjk.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hee.yangfankeji.com

[Q63] 开启事务
来源：http://bus.yuanzhike.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jxa.9152youxi.cn

[Q64] 提交事务
来源：http://lmr.smart0.xyz

COMMIT;
来源：http://lww.meibo888.top

[Q65] 回滚事务
来源：http://mjq.hywenlv.cn

ROLLBACK;
来源：http://kaz.xuetiantiany.cn

[Q66] 行锁查询
来源：http://wwo.yonumen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lzx.vqdsnc.cn

[Q67] 设置隔离级别
来源：http://ffa.zhongyouzk.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iua.chenjidiqi.icu

[Q68] 保存点
来源：http://dco.zhongyouzk.top

SAVEPOINT sp1;
来源：http://mxq.nwbrower.top

ROLLBACK TO sp1;
来源：http://ler.guowangkeji.top

[Q69] 查看执行计划
来源：http://dki.fengsongda.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zbm.redwolf501.top

[Q70] 更新统计信息
来源：http://qsq.haohaochexian.top

ANALYZE TABLE users;
来源：http://fwk.ydzc1.top

[Q71] 查看建表语句
来源：http://oqt.smart0.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hfh.vqdsnc.cn

[Q72] 查看索引
来源：http://ouo.smart0.xyz

SHOW INDEX FROM users;
来源：http://poc.dianchejie.cn

[Q73] 查看表状态
来源：http://cal.fzhhl.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ezw.zycfv.cn

[Q74] 强制使用索引
来源：http://uyd.hysaishi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vgy.jiagoushi.top

[Q75] 日期格式化
来源：http://wgd.nanxinkj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cma.yfazqb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yoo.wangshuangyany.cn

[Q76] 按天统计
来源：http://keo.nanxinkj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xdf.hongshengwenyu.top

[Q77] 时间加减
来源：http://tem.cheryme.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mft.ivvv.top

[Q78] 当前时间
来源：http://jzy.shzxlz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kvv.yj202588.top

[Q79] 字符串拼接
来源：http://pth.ybcxt.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://coq.tarul.cn

[Q80] 字符串截取
来源：http://cvj.jinyuanbaomall.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://awj.dianchejie.cn

[Q81] 字符串替换
来源：http://juf.xuetiantiany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wru.uphjek.com

[Q82] 字符长度与字节长度
来源：http://ffc.shanyushiyangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rze.yfazqb.com

[Q83] 大小写转换
来源：http://igs.sxryk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tjr.tanke756.top

[Q84] 去除首尾空格
来源：http://uoc.bjfxy.top

SELECT TRIM(name) FROM users;
来源：http://zzj.chenlongwang.top

[Q85] 数值取整
来源：http://idi.hnxiangtu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bwx.haohaochexian.top

[Q86] 读取 JSON 字段
来源：http://vax.vehdjk.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yyy.cheryme.top

[Q87] JSON 字段做条件
来源：http://wsr.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qcy.yonumen.top

[Q88] 行转列（条件聚合）
来源：http://ssr.gogol.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lev.chenzaomai.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://msc.xingfuxueyuan.xyz

[Q89] 判断表是否存在
来源：http://fai.redwolf501.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mnk.zhoulong.xyz

[Q90] 生成序号列
来源：http://atk.yueranfly.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fnb.cheryme.top

================================================================================
来源：http://awj.yfazqb.com

R. Bash 专题
来源：http://pkl.wangshuangyany.cn

================================================================================
来源：http://wur.gzhubu.top

[R01] shebang 与严格模式
来源：http://yyw.wangdashe.top

#!/usr/bin/env bash
来源：http://cbm.yueranfly.top

set -euo pipefail
来源：http://ppm.guowangkeji.top

[R02] 变量赋值与使用
来源：http://nmm.zdqjudy.top

name="Tom"; echo "$name"
来源：http://uez.havefunace.top

[R03] 只读变量
来源：http://zpl.yj202588.top

readonly PI=3.14
来源：http://pyi.zhengqikj.top

[R04] 位置参数
来源：http://dne.iojbl.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sdn.shanyushiyangtech.top

[R05] 参数默认值
来源：http://kxb.daxiang520.top

name="${1:-default}"
来源：http://hsa.tian-w.cn

[R06] 判断命令是否存在
来源：http://fpt.nanxuanxn.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://knw.svipenyu.cn

[R07] if 判断文件
来源：http://cno.zycfv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eqc.ybcxt.top

[R08] 数值比较
来源：http://bsw.hysaishi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://aye.fengsongda.top

[R09] 字符串比较
来源：http://cxo.birdmap.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bqh.shanyushiyangkeji.top

[R10] 正则匹配
来源：http://hym.hnqzz.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yip.zycfv.cn

[R11] case 多分支
来源：http://yhp.tarul.cn

case "$1" in
来源：http://xtx.wangshuangyany.cn

start) echo "启动" ;;
来源：http://ibx.sweek.top

stop)  echo "停止" ;;
来源：http://btv.ywan-chungtsiang.top

*)     echo "未知命令" ;;
来源：http://gcx.dianchejie.cn

esac
来源：http://vkv.xziqi.cn

[R12] for 遍历文件
来源：http://dxr.316326.xyz

for f in *.txt; do echo "$f"; done
来源：http://jzr.xziqi.cn

[R13] for 计数循环
来源：http://lfe.shangyingyoupin.top

for i in {1..10}; do echo "$i"; done
来源：http://nba.kuanghao11.cn

[R14] C 风格 for
来源：http://rxk.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lsw.yj20258.top

[R15] while 逐行读文件
来源：http://god.tianlin.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lgy.yuanzhike.top

[R16] until 等待条件
来源：http://atv.ydjk.org.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zcj.jiagoushi.top

[R17] 数组定义与取值
来源：http://muo.gaohongyu789.top

arr=(a b c); echo "${arr[0]}"
来源：http://jcp.tarul.cn

[R18] 遍历数组
来源：http://vyp.guowangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kti.gotoacloud.top

[R19] 数组长度
来源：http://ams.hywenlv.cn

echo "${#arr[@]}"
来源：http://xhz.vehdjk.com

[R20] 关联数组（字典）
来源：http://fiv.snrcjt.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ccm.aizwys.cn

[R21] 字符串长度
来源：http://rfr.ydzc1.top

echo "${#s}"
来源：http://gcl.hcnkem.com

[R22] 截取子串
来源：http://mfx.shzxlz.cn

echo "${s:0:5}"
来源：http://ykm.jinqigfzy.top

[R23] 字符串替换
来源：http://jxa.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gak.dianchejie.cn

[R24] 大小写转换
来源：http://wid.hcnkem.com

echo "${s^^}"; echo "${s,,}"
来源：http://kjf.cucudq.cn

[R25] 去后缀 / 去前缀
来源：http://qen.xingfuxueyuan.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://lvp.tian-w.cn

[R26] 命令替换
来源：http://htw.zhixingplan.top

now=$(date +%F); echo "$now"
来源：http://eto.tian-w.cn

[R27] 算术展开
来源：http://wvy.xylfe.cn

echo $((1 + 2 * 3))
来源：http://xsk.52xcode.cn

[R28] 浮点运算
来源：http://oce.ehwqpu.com

echo "scale=2; 10/3" | bc
来源：http://jqj.bjfxy.top

[R29] 定义函数
来源：http://vfr.zhoulong.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bbg.shanyushiyangkeji.top

[R30] 函数返回状态码
来源：http://iyw.svipenyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://ema.cucudq.cn

[R31] 局部变量
来源：http://foy.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://dzx.fengsongda.top

[R32] 参数个数校验
来源：http://jiz.yj20258.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ila.sysykeji.top

[R33] 捕获错误并提示行号
来源：http://nio.9152youxi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wor.chenlongwang.top

[R34] 退出时清理
来源：http://huh.svipenyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ilh.chenlongwang.top

[R35] 后台执行并等待
来源：http://doi.xuanzx.com

sleep 5 & pid=$!; wait "$pid"
来源：http://lsg.mhx1999.top

[R36] 并发执行多个任务
来源：http://smx.gzhubu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://snx.nanxinkj.top

[R37] 把输出赋给变量
来源：http://ubn.epnwcf.com

files=$(ls -1)
来源：http://rmf.xylfe.cn

[R38] 管道串联
来源：http://qsv.hfpthk.cn

cat a.txt | grep -i error | wc -l
来源：http://rto.sxryk.cn

[R39] 重定向标准输出与错误
来源：http://bdi.52xcode.cn

cmd > out.log 2>&1
来源：http://kyb.smart0.xyz

[R40] 追加写日志
来源：http://wrn.zhongyouzk.top

echo "log" >> out.log
来源：http://tqx.cdnleiting.top

[R41] 丢弃输出
来源：http://iwg.zhijiandao.cn

cmd >/dev/null 2>&1
来源：http://yyg.c1oappe.top

[R42] 输入重定向
来源：http://ufk.chenjidiqi.icu

wc -l < a.txt
来源：http://bja.dashuyun.cn

[R43] 按名字查找文件
来源：http://erg.chenzaomai.com

find . -name "*.log" -type f
来源：http://vvz.dianchejie.cn

[R44] 按修改时间查找
来源：http://lgd.c1oappe.top

find . -mtime -7 -type f
来源：http://irl.cucudq.cn

[R45] 批量删除
来源：http://mhp.birdmap.top

find . -name "*.tmp" -delete
来源：http://hmd.xylfe.cn

[R46] 递归替换文件内容
来源：http://lzs.tianlin.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://elo.yfazqb.com

[R47] sed 单行替换
来源：http://sgd.tarul.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zfb.cashguo.top

[R48] awk 取指定列
来源：http://ynx.zycfv.cn

awk '{print $1, $3}' a.txt
来源：http://rgr.yfazqb.com

[R49] awk 带条件
来源：http://gtn.jqgfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sfu.hnxiangtu.top

[R50] awk 求和
来源：http://fex.tian-w.cn

awk '{s += $2} END {print s}' a.txt
来源：http://prd.meibo888.top

[R51] 排序去重取前几
来源：http://nbc.snrcjt.cn


<!-- 参考信息 -->