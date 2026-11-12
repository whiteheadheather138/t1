代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://jqs.tian-w.cn

[Q07] 删除表
来源：http://csm.sjlbkw.cn

DROP TABLE IF EXISTS orders;
来源：http://zcd.wangdashe.top

[Q08] 创建普通索引
来源：http://lno.chenlongwang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://tze.tarul.cn

[Q09] 创建唯一索引
来源：http://uzm.zycfv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://btp.zhijiandao.cn

[Q10] 插入单行
来源：http://aay.jinqigfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ofm.fengsongda.top

[Q11] 一次插入多行
来源：http://cey.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nno.jiagoushi.top

[Q12] 插入后取自增 ID
来源：http://hgm.aibaodan.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tvk.jqgfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://emc.svipenyu.cn

[Q13] 忽略重复插入
来源：http://pho.jinqigfzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://snv.zhengqikj.top

[Q14] 存在则更新（upsert）
来源：http://zer.uphjek.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bfn.zycfv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://shq.shangyingyoupin.top

[Q15] 查询全部
来源：http://cgx.haohaochexian.top

SELECT * FROM users;
来源：http://jnn.smart0.xyz

[Q16] 查询指定列
来源：http://rlb.sufxvd.cn

SELECT id, name FROM users;
来源：http://wlb.kuanghao11.cn

[Q17] 条件查询
来源：http://rkk.havefunace.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qqf.chenzaomai.com

[Q18] 模糊匹配
来源：http://gwr.ywan-chungtsiang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rmq.52xcode.cn

[Q19] 范围查询
来源：http://whn.jinqigufen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wsh.xylfe.cn

[Q20] IN 列表
来源：http://isr.ehwqpu.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tbq.fengsongda.top

[Q21] 空值判断
来源：http://otx.redwolf501.top

SELECT * FROM users WHERE email IS NULL;
来源：http://cbw.ppjwa.cn

[Q22] 排序
来源：http://plc.yj202588.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://obe.jianghu66.top

[Q23] 分页
来源：http://rox.fzhhl.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wfv.bjfxy.top

[Q24] 去重
来源：http://caw.zycfv.cn

SELECT DISTINCT city FROM users;
来源：http://tgg.fehbvm.com

[Q25] 只取前 N 条
来源：http://tvm.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tid.yuxming.cn

[Q26] 计数
来源：http://dap.hfpthk.cn

SELECT COUNT(*) FROM users;
来源：http://cak.zhaomingkeji.xyz

[Q27] 条件计数
来源：http://xqn.xuanzx.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://viv.aibaodan.cn

[Q28] 求和与平均
来源：http://wkn.zycfv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mbs.nanxinkj.top

[Q29] 最大最小值
来源：http://glz.zhiwuduotai.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://kxt.jianghu66.top

[Q30] 分组统计
来源：http://qjm.yj202588.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yzq.c1oappe.top

[Q31] 分组后过滤
来源：http://dnt.feifeiyinyue.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://udb.9152youxi.cn

[Q32] 分组拼接字符串
来源：http://vmc.hammf.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mqc.fktsv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lwz.fengsongda.top

[Q33] 多列分组
来源：http://cjp.vehdjk.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sjw.chenjidiqi.icu

[Q34] 每组取第一条
来源：http://auz.zhoulong.xyz

SELECT * FROM (
来源：http://rqk.ybcxt.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zbw.vqdsnc.cn

) t WHERE rn = 1;
来源：http://mwz.jinghuilouyu.cn

[Q35] 内连接
来源：http://aae.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fmf.daria6918.cn

[Q36] 左连接
来源：http://ahv.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tsw.ydjk.org.cn

[Q37] 右连接
来源：http://xbe.zdbjq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://upc.tarul.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mrb.dianchejie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pet.guowangkeji.top

[Q39] 自连接（查上下级）
来源：http://scv.jlsjyb.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wlg.haohaochexian.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://obx.zhixingplan.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vdi.yfazqb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://joq.snrcjt.cn

[Q41] 多表连接
来源：http://svf.cqqwz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mko.sxryk.cn

JOIN users u ON u.id = o.user_id
来源：http://npi.ivvv.top

JOIN products p ON p.id = o.product_id;
来源：http://qnk.snrcjt.cn

[Q42] 连接条件附加过滤
来源：http://mmy.jlsjyb.cn

SELECT u.name, o.amount FROM users u
来源：http://uzq.ctjpmb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xis.uphjek.com

[Q43] 标量子查询
来源：http://zpx.jinyuanbaomall.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://owk.gotoacloud.top

[Q44] IN 子查询
来源：http://waf.epnwcf.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qmj.fktsv.cn

[Q45] EXISTS 判断存在
来源：http://idp.ehwqpu.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ovl.jqgfzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://xmu.hfpthk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bso.jinyuanbaomall.cn

[Q47] 与平均值比较
来源：http://kvl.zhaomingkeji.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sct.uphjek.com

[Q48] CTE 公用表表达式
来源：http://hit.andypj.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://llj.fengsongda.top

SELECT * FROM t WHERE c > 5;
来源：http://qst.fehbvm.com

[Q49] 更新单行
来源：http://fuf.guannengcc.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sey.tanke756.top

[Q50] 批量更新
来源：http://gsp.hammf.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kxc.feifeiyinyue.top

[Q51] 用子查询更新
来源：http://axw.xingfuxueyuan.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dty.nanxinkj.top

[Q52] 删除指定行
来源：http://fmi.cashguo.top

DELETE FROM users WHERE id = 10;
来源：http://gjx.zdbjq.cn

[Q53] 按条件删除
来源：http://pnm.jiagoushi.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qds.redwolf501.top

[Q54] 清空表
来源：http://nxh.bjfxy.top

TRUNCATE TABLE logs;
来源：http://mfa.zhoulong.xyz

[Q55] 排名（并列占位）
来源：http://sxt.gogol.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rci.hfpthk.cn

[Q56] 密集排名（并列不占位）
来源：http://ksj.daria6918.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qrf.xuanzx.com

[Q57] 行号
来源：http://hxv.fehbvm.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://llv.zdqjudy.top

[Q58] 累计求和
来源：http://jjz.chenlongwang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wkc.hysaishi.cn

[Q59] 分组内累计
来源：http://ouy.yueranfly.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zjb.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://sib.pycfn.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ygz.jinghuilouyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gtd.zhoulong.xyz

[Q61] 移动平均
来源：http://chy.uphjek.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jrk.c1oappe.top

[Q62] 分组占比
来源：http://qzo.jinghuilouyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oas.yueranfly.top

[Q63] 开启事务
来源：http://opd.zhijiandao.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zjv.andypj.xyz

[Q64] 提交事务
来源：http://wst.ydzc1.top

COMMIT;
来源：http://nah.gogol.net.cn

[Q65] 回滚事务
来源：http://uzv.fanxiaobao.xyz

ROLLBACK;
来源：http://ana.daxiang520.top

[Q66] 行锁查询
来源：http://zwk.jyoumei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://apg.yueranfly.top

[Q67] 设置隔离级别
来源：http://ioq.pycfn.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://aod.yvedp.cn

[Q68] 保存点
来源：http://krd.dianchejie.cn

SAVEPOINT sp1;
来源：http://rbs.shangyingyoupin.top

ROLLBACK TO sp1;
来源：http://qyk.epnwcf.com

[Q69] 查看执行计划
来源：http://cfh.quarkkingdee.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fft.yongpay.top

[Q70] 更新统计信息
来源：http://mkd.mhx1999.top

ANALYZE TABLE users;
来源：http://eez.vehdjk.com

[Q71] 查看建表语句
来源：http://tpx.jinqigufen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wgc.mhx1999.top

[Q72] 查看索引
来源：http://bvf.cucudq.cn

SHOW INDEX FROM users;
来源：http://pak.zdqjudy.top

[Q73] 查看表状态
来源：http://zgl.yfazqb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://pgd.shangyingyoupin.top

[Q74] 强制使用索引
来源：http://mnr.sxryk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fdq.uphjek.com

[Q75] 日期格式化
来源：http://sje.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bao.zhongyouzk.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sgz.kuanghao11.cn

[Q76] 按天统计
来源：http://xuf.shuidangran.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://czr.yvedp.cn

[Q77] 时间加减
来源：http://ceh.pengpengdd.cyou

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://odd.jianghu66.top

[Q78] 当前时间
来源：http://gge.dianchejie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jeh.hfpthk.cn

[Q79] 字符串拼接
来源：http://lnv.gzhubu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://unq.snrcjt.cn

[Q80] 字符串截取
来源：http://ydz.iojbl.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iud.zhoulong.xyz

[Q81] 字符串替换
来源：http://qun.jinqigufen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qun.shanyushiyangkeji.top

[Q82] 字符长度与字节长度
来源：http://xjx.tanke756.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ozp.sxryk.cn

[Q83] 大小写转换
来源：http://mta.yangfankeji.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yrl.tanke756.top

[Q84] 去除首尾空格
来源：http://ege.tarul.cn

SELECT TRIM(name) FROM users;
来源：http://ydt.bbcook.cn

[Q85] 数值取整
来源：http://jhu.hesvh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nht.zdbjq.cn

[Q86] 读取 JSON 字段
来源：http://jxh.fzhhl.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wzm.xuanzx.com

[Q87] JSON 字段做条件
来源：http://yaq.sxryk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zsh.daria6918.cn

[Q88] 行转列（条件聚合）
来源：http://ljk.gotoacloud.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zwk.fanxiaobao.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jbu.iojbl.cn

[Q89] 判断表是否存在
来源：http://fdz.zdbjq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ung.snrcjt.cn

[Q90] 生成序号列
来源：http://gdy.yuxming.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://scl.jiagoushi.top

================================================================================
来源：http://ncu.nwbrower.top

R. Bash 专题
来源：http://kmn.xingfuxueyuan.xyz

================================================================================
来源：http://tgq.yangfankeji.com

[R01] shebang 与严格模式
来源：http://vpv.shanyushiyangtech.top

#!/usr/bin/env bash
来源：http://oky.jianghu66.top

set -euo pipefail
来源：http://pit.cqqwz.cn

[R02] 变量赋值与使用
来源：http://hzy.jqgfzy.top

name="Tom"; echo "$name"
来源：http://svs.cheryme.top

[R03] 只读变量
来源：http://nci.jinghuilouyu.cn

readonly PI=3.14
来源：http://sql.zdbjq.cn

[R04] 位置参数
来源：http://hbs.svipenyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://adq.nanxinkj.top

[R05] 参数默认值
来源：http://qol.zhaomingkeji.xyz

name="${1:-default}"
来源：http://cnl.ivvv.top

[R06] 判断命令是否存在
来源：http://wrh.tianlin.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hey.daxiang520.top

[R07] if 判断文件
来源：http://bix.jinyuanbaomall.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://und.nanxinkj.top

[R08] 数值比较
来源：http://zii.cucudq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lbk.nanxinkj.top

[R09] 字符串比较
来源：http://rqv.ybcxt.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jej.hcnkem.com

[R10] 正则匹配
来源：http://wqc.hnxiangtu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://twm.sysykeji.top

[R11] case 多分支
来源：http://mcl.xinyue.icu

case "$1" in
来源：http://koe.jiagoushi.top

start) echo "启动" ;;
来源：http://dwu.yuxming.cn

stop)  echo "停止" ;;
来源：http://xli.yanxiufei.cn

*)     echo "未知命令" ;;
来源：http://vbj.hywenlv.cn

esac
来源：http://zyj.tianlin.xyz

[R12] for 遍历文件
来源：http://eva.jyoumei.cn

for f in *.txt; do echo "$f"; done
来源：http://poi.iojbl.cn

[R13] for 计数循环
来源：http://jog.fzhhl.top

for i in {1..10}; do echo "$i"; done
来源：http://ayo.havefunace.top

[R14] C 风格 for
来源：http://rpg.shanyushiyangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://igo.fzhhl.top

[R15] while 逐行读文件
来源：http://blf.hesvh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mqc.yj20258888.top

[R16] until 等待条件
来源：http://aba.shangyingyoupin.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wdn.guowangkeji.top

[R17] 数组定义与取值
来源：http://hff.birdmap.top

arr=(a b c); echo "${arr[0]}"
来源：http://ueb.cashguo.top

[R18] 遍历数组
来源：http://rgv.yj20258888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iur.ywan-chungtsiang.top

[R19] 数组长度
来源：http://ysw.aizwys.cn

echo "${#arr[@]}"
来源：http://vsb.9152youxi.cn

[R20] 关联数组（字典）
来源：http://dfm.yonumen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://owy.316326.xyz

[R21] 字符串长度
来源：http://vuo.zhiwuduotai.top

echo "${#s}"
来源：http://lya.nanxinkj.top

[R22] 截取子串
来源：http://ifo.gogol.net.cn

echo "${s:0:5}"
来源：http://oic.zhoulong.xyz

[R23] 字符串替换
来源：http://ylu.quarkkingdee.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bqe.ivvv.top

[R24] 大小写转换
来源：http://exe.zhijiandao.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xzz.vqdsnc.cn

[R25] 去后缀 / 去前缀
来源：http://rej.daria6918.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ycj.vqdsnc.cn

[R26] 命令替换
来源：http://ajt.jianghu66.top

now=$(date +%F); echo "$now"
来源：http://tgl.ydjk.org.cn

[R27] 算术展开
来源：http://fhu.chenzaomai.com

echo $((1 + 2 * 3))
来源：http://szz.sxryk.cn

[R28] 浮点运算
来源：http://tih.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://den.9152youxi.cn

[R29] 定义函数
来源：http://zjd.fehbvm.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xzr.aizwys.cn

[R30] 函数返回状态码
来源：http://vwa.snrcjt.cn

f() { return 0; }; f || echo "失败了"
来源：http://kxt.haohaochexian.top

[R31] 局部变量
来源：http://ecl.xylfe.cn

f() { local x=1; echo "$x"; }
来源：http://azi.pengpengdd.cyou

[R32] 参数个数校验
来源：http://sks.kuanghao11.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xyw.316326.xyz

[R33] 捕获错误并提示行号
来源：http://lif.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pyk.mhx1999.top

[R34] 退出时清理
来源：http://snb.zdbjq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ebk.xuanzx.com

[R35] 后台执行并等待
来源：http://wbd.bjfxy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qzg.ydzc1.top

[R36] 并发执行多个任务
来源：http://xtg.gzhubu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qtp.meibo888.top

[R37] 把输出赋给变量
来源：http://dvq.kuanghao11.cn

files=$(ls -1)
来源：http://doj.fehbvm.com

[R38] 管道串联
来源：http://xst.ctjpmb.com

cat a.txt | grep -i error | wc -l
来源：http://yrt.fehbvm.com

[R39] 重定向标准输出与错误
来源：http://hev.xziqi.cn

cmd > out.log 2>&1
来源：http://vwe.gotoacloud.top

[R40] 追加写日志
来源：http://sjc.haohaochexian.top

echo "log" >> out.log
来源：http://yqw.yj20258.top

[R41] 丢弃输出
来源：http://hfg.zycfv.cn

cmd >/dev/null 2>&1
来源：http://sfq.kuanghao11.cn

[R42] 输入重定向
来源：http://fkx.9152youxi.cn

wc -l < a.txt
来源：http://nnr.feifeiyinyue.top

[R43] 按名字查找文件
来源：http://wvp.zhoulong.xyz

find . -name "*.log" -type f
来源：http://tir.aizwys.cn

[R44] 按修改时间查找
来源：http://ihc.sweek.top

find . -mtime -7 -type f
来源：http://xic.ybcxt.top

[R45] 批量删除
来源：http://azg.jqgfzy.top

find . -name "*.tmp" -delete
来源：http://mwd.meibo888.top

[R46] 递归替换文件内容
来源：http://opp.pycfn.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fti.jianghu66.top

[R47] sed 单行替换
来源：http://ljj.chenjidiqi.icu

sed -i 's/foo/bar/g' a.txt
来源：http://qei.mhx1999.top

[R48] awk 取指定列
来源：http://gbk.sjlbkw.cn

awk '{print $1, $3}' a.txt
来源：http://fjf.smart0.xyz

[R49] awk 带条件
来源：http://lhi.zhijiandao.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ujg.pycfn.com

[R50] awk 求和
来源：http://tgw.ctjpmb.com

awk '{s += $2} END {print s}' a.txt
来源：http://nso.ehwqpu.com

[R51] 排序去重取前几
来源：http://dcf.hfpthk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bfn.yj20258.top

[R52] 统计行数
来源：http://zgo.shanyushiyangtech.top

wc -l a.txt
来源：http://xid.c1oappe.top

[R53] 查看文件头与实时尾
来源：http://ani.havefunace.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mqg.yj202588.top

[R54] 比较两个文件
来源：http://riu.bjfxy.top

diff a.txt b.txt
来源：http://lsg.fengsongda.top

[R55] 压缩与解压
来源：http://kjt.hammf.cn


<!-- 参考信息 -->