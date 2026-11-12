代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://mbh.fengsongda.top

[Q09] 创建唯一索引
来源：http://ghy.sysykeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vqe.sysykeji.top

[Q10] 插入单行
来源：http://nba.yongpay.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yxo.xylfe.cn

[Q11] 一次插入多行
来源：http://gxc.sweek.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lsb.yonumen.top

[Q12] 插入后取自增 ID
来源：http://uth.fengsongda.top

INSERT INTO users (name) VALUES ('C');
来源：http://ztg.feifeiyinyue.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ntq.sweek.top

[Q13] 忽略重复插入
来源：http://bgg.feifeiyinyue.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wnf.shzxlz.cn

[Q14] 存在则更新（upsert）
来源：http://cyn.cheryme.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ihq.fehbvm.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ypq.shanyushiyangkeji.top

[Q15] 查询全部
来源：http://nsr.dashuyun.cn

SELECT * FROM users;
来源：http://rlw.chenjidiqi.icu

[Q16] 查询指定列
来源：http://yrx.jqgfzy.top

SELECT id, name FROM users;
来源：http://pyz.ywan-chungtsiang.top

[Q17] 条件查询
来源：http://ade.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sqm.hesvh.cn

[Q18] 模糊匹配
来源：http://gsp.wangdashe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://csg.hesvh.cn

[Q19] 范围查询
来源：http://yiy.fanxiaobao.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mnp.epnwcf.com

[Q20] IN 列表
来源：http://aif.quarkkingdee.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xyi.daxiang520.top

[Q21] 空值判断
来源：http://yik.0kj1m.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zbt.jyoumei.cn

[Q22] 排序
来源：http://tds.yj202588.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qpe.yanxiufei.cn

[Q23] 分页
来源：http://xkl.fanxiaobao.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vai.zhongyouzk.top

[Q24] 去重
来源：http://tlp.jqgufenzy.top

SELECT DISTINCT city FROM users;
来源：http://jfd.xylfe.cn

[Q25] 只取前 N 条
来源：http://eaz.shanyushiyangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pua.daxiang520.top

[Q26] 计数
来源：http://upa.yj20258.top

SELECT COUNT(*) FROM users;
来源：http://tyl.gzhubu.top

[Q27] 条件计数
来源：http://pno.ppjwa.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jxi.jqgfzy.top

[Q28] 求和与平均
来源：http://fag.nanxuanxn.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ekk.daxiang520.top

[Q29] 最大最小值
来源：http://qvz.birdmap.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://erd.aizwys.cn

[Q30] 分组统计
来源：http://nff.zhengqikj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mmz.xylfe.cn

[Q31] 分组后过滤
来源：http://aqv.shuidangran.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ptg.bbcook.cn

[Q32] 分组拼接字符串
来源：http://eyw.aibaodan.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xyg.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://umy.gogol.net.cn

[Q33] 多列分组
来源：http://tgh.sufxvd.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://efa.redwolf501.top

[Q34] 每组取第一条
来源：http://fmb.zhongyouzk.top

SELECT * FROM (
来源：http://qjd.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wkx.chenjidiqi.icu

) t WHERE rn = 1;
来源：http://uhu.hnqzz.top

[Q35] 内连接
来源：http://qwt.quarkkingdee.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ryx.birdmap.top

[Q36] 左连接
来源：http://pqr.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tmx.nanxuanxn.top

[Q37] 右连接
来源：http://ksd.bjfxy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uni.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yko.ydjk.org.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zvf.shanyushiyangtech.top

[Q39] 自连接（查上下级）
来源：http://rwm.sxryk.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bsv.hnqzz.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lhi.cheryme.top

[Q40] 交叉连接（笛卡尔积）
来源：http://eks.0kj1m.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yde.yongpay.top

[Q41] 多表连接
来源：http://fli.chenzaomai.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://kxh.zhengqikj.top

JOIN users u ON u.id = o.user_id
来源：http://rjt.gzhubu.top

JOIN products p ON p.id = o.product_id;
来源：http://aqk.aizwys.cn

[Q42] 连接条件附加过滤
来源：http://zkd.sweek.top

SELECT u.name, o.amount FROM users u
来源：http://gnb.shzxlz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mwg.quarkkingdee.top

[Q43] 标量子查询
来源：http://fqw.yueranfly.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sfr.hesvh.cn

[Q44] IN 子查询
来源：http://sbp.tarul.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://boc.xuetiantiany.cn

[Q45] EXISTS 判断存在
来源：http://wbw.iojbl.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wue.xylfe.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xkh.dianchejie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qxx.redwolf501.top

[Q47] 与平均值比较
来源：http://hor.vehdjk.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ycf.uphjek.com

[Q48] CTE 公用表表达式
来源：http://fsk.yueranfly.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ezu.sysykeji.top

SELECT * FROM t WHERE c > 5;
来源：http://tdy.jqgufenzy.top

[Q49] 更新单行
来源：http://yza.kuanghao11.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ona.jianghu66.top

[Q50] 批量更新
来源：http://zdx.yuxming.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fvt.zhoulong.xyz

[Q51] 用子查询更新
来源：http://dye.ydjk.org.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oud.guannengcc.top

[Q52] 删除指定行
来源：http://ata.hcnkem.com

DELETE FROM users WHERE id = 10;
来源：http://hke.daxiang520.top

[Q53] 按条件删除
来源：http://kvo.pengpengdd.cyou

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://orv.zhengqikj.top

[Q54] 清空表
来源：http://qyn.tarul.cn

TRUNCATE TABLE logs;
来源：http://det.pycfn.com

[Q55] 排名（并列占位）
来源：http://xbc.ywan-chungtsiang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bom.uphjek.com

[Q56] 密集排名（并列不占位）
来源：http://lfu.cucudq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mye.shzxlz.cn

[Q57] 行号
来源：http://hdd.meibo888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ghi.jinyuanbaomall.cn

[Q58] 累计求和
来源：http://tnm.jqgufenzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jnq.sjlbkw.cn

[Q59] 分组内累计
来源：http://yed.shanyushiyangkeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://azi.yuanzhike.top

[Q60] 取上一行 / 下一行
来源：http://ofr.tian-w.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dos.yj202588.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ptz.sysykeji.top

[Q61] 移动平均
来源：http://gyo.yj20258888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dlk.xylfe.cn

[Q62] 分组占比
来源：http://hsz.xylfe.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xqj.andypj.xyz

[Q63] 开启事务
来源：http://ysk.ivvv.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tyn.ctjpmb.com

[Q64] 提交事务
来源：http://jub.andypj.xyz

COMMIT;
来源：http://jiv.hywenlv.cn

[Q65] 回滚事务
来源：http://czz.fehbvm.com

ROLLBACK;
来源：http://pid.zhengqikj.top

[Q66] 行锁查询
来源：http://dgt.redwolf501.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ekk.xuanzx.com

[Q67] 设置隔离级别
来源：http://bxo.hnqzz.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sai.xylfe.cn

[Q68] 保存点
来源：http://ens.wangdashe.top

SAVEPOINT sp1;
来源：http://ohx.xinyue.icu

ROLLBACK TO sp1;
来源：http://tnr.tanke756.top

[Q69] 查看执行计划
来源：http://uob.daria6918.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pgw.yangfankeji.com

[Q70] 更新统计信息
来源：http://jnh.cheryme.top

ANALYZE TABLE users;
来源：http://zuf.kuanghao11.cn

[Q71] 查看建表语句
来源：http://axt.hammf.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tcg.yuanzhike.top

[Q72] 查看索引
来源：http://epi.xinyue.icu

SHOW INDEX FROM users;
来源：http://aam.316326.xyz

[Q73] 查看表状态
来源：http://sef.zhixingplan.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zjs.yfazqb.com

[Q74] 强制使用索引
来源：http://vca.iojbl.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://adu.hesvh.cn

[Q75] 日期格式化
来源：http://zyp.shzxlz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zja.gogol.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://syr.yvedp.cn

[Q76] 按天统计
来源：http://kpo.shzxlz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://byg.bbcook.cn

[Q77] 时间加减
来源：http://bps.quarkkingdee.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://chi.sweek.top

[Q78] 当前时间
来源：http://htc.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rpw.c1oappe.top

[Q79] 字符串拼接
来源：http://oei.daxiang520.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ovg.9152youxi.cn

[Q80] 字符串截取
来源：http://qol.epnwcf.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ypg.fehbvm.com

[Q81] 字符串替换
来源：http://ibg.tianlin.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yna.cashguo.top

[Q82] 字符长度与字节长度
来源：http://ifc.redwolf501.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yuq.yj20258888.top

[Q83] 大小写转换
来源：http://ygz.jinqigufen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gtt.xinyue.icu

[Q84] 去除首尾空格
来源：http://mdy.jiagoushi.top

SELECT TRIM(name) FROM users;
来源：http://isk.shanyushiyangkeji.top

[Q85] 数值取整
来源：http://pyo.gotoacloud.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ttm.zhengqikj.top

[Q86] 读取 JSON 字段
来源：http://hnm.quarkkingdee.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fff.bjfxy.top

[Q87] JSON 字段做条件
来源：http://bnp.gotoacloud.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://opp.cheryme.top

[Q88] 行转列（条件聚合）
来源：http://naa.9152youxi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zst.cucudq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ylo.vqdsnc.cn

[Q89] 判断表是否存在
来源：http://mkb.gzhubu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nyn.hcnkem.com

[Q90] 生成序号列
来源：http://anr.ydjk.org.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nfw.zhaomingkeji.xyz

================================================================================
来源：http://cza.cashguo.top

R. Bash 专题
来源：http://znv.tian-w.cn

================================================================================
来源：http://smg.shuidangran.top

[R01] shebang 与严格模式
来源：http://oxr.daria6918.cn

#!/usr/bin/env bash
来源：http://imv.aibaodan.cn

set -euo pipefail
来源：http://wge.ivvv.top

[R02] 变量赋值与使用
来源：http://frt.hysaishi.cn

name="Tom"; echo "$name"
来源：http://bez.c1oappe.top

[R03] 只读变量
来源：http://rxz.cdnleiting.top

readonly PI=3.14
来源：http://ocx.hammf.cn

[R04] 位置参数
来源：http://ere.epnwcf.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yoy.hesvh.cn

[R05] 参数默认值
来源：http://drb.52xcode.cn

name="${1:-default}"
来源：http://mkk.fzhhl.top

[R06] 判断命令是否存在
来源：http://hpf.tianlin.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nam.yj202588.top

[R07] if 判断文件
来源：http://hpa.wangshuangyany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zhy.zhongyouzk.top

[R08] 数值比较
来源：http://gsn.yfazqb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://hjz.vqdsnc.cn

[R09] 字符串比较
来源：http://mnp.xuanzx.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aox.yueranfly.top

[R10] 正则匹配
来源：http://kfb.kuanghao11.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mhq.shangyingyoupin.top

[R11] case 多分支
来源：http://res.feifeiyinyue.top

case "$1" in
来源：http://mjf.sysykeji.top

start) echo "启动" ;;
来源：http://ldn.hongshengwenyu.top

stop)  echo "停止" ;;
来源：http://jzt.ybcxt.top

*)     echo "未知命令" ;;
来源：http://vys.chenlongwang.top

esac
来源：http://kuw.gzhubu.top

[R12] for 遍历文件
来源：http://yjq.epnwcf.com

for f in *.txt; do echo "$f"; done
来源：http://ldu.wangshuangyany.cn

[R13] for 计数循环
来源：http://gme.yvedp.cn

for i in {1..10}; do echo "$i"; done
来源：http://afj.guannengcc.top

[R14] C 风格 for
来源：http://ghm.chenlongwang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vnx.0kj1m.cn

[R15] while 逐行读文件
来源：http://xsw.havefunace.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mlj.daxiang520.top

[R16] until 等待条件
来源：http://ywi.xinyue.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://edf.zhixingplan.top

[R17] 数组定义与取值
来源：http://zws.sufxvd.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cdp.zycfv.cn

[R18] 遍历数组
来源：http://lip.jyoumei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://feo.cheryme.top

[R19] 数组长度
来源：http://bbc.ydjk.org.cn

echo "${#arr[@]}"
来源：http://mcx.jinqigufen.top

[R20] 关联数组（字典）
来源：http://eut.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kih.vqdsnc.cn

[R21] 字符串长度
来源：http://esr.xziqi.cn

echo "${#s}"
来源：http://btd.sxryk.cn

[R22] 截取子串
来源：http://war.guowangkeji.top

echo "${s:0:5}"
来源：http://vvc.fzhhl.top

[R23] 字符串替换
来源：http://gkl.snrcjt.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://asd.sufxvd.cn

[R24] 大小写转换
来源：http://gho.hnqzz.top

echo "${s^^}"; echo "${s,,}"
来源：http://jxn.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://zfx.zhengqikj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fim.epnwcf.com

[R26] 命令替换
来源：http://znx.jianghu66.top

now=$(date +%F); echo "$now"
来源：http://jhu.xylfe.cn

[R27] 算术展开
来源：http://thc.cheryme.top

echo $((1 + 2 * 3))
来源：http://rpb.cdnleiting.top

[R28] 浮点运算
来源：http://uhi.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://itd.iojbl.cn

[R29] 定义函数
来源：http://hln.guowangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qeu.hnxiangtu.top

[R30] 函数返回状态码
来源：http://jrf.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://azk.shuidangran.top

[R31] 局部变量
来源：http://ipk.guowangkeji.top

f() { local x=1; echo "$x"; }
来源：http://ipm.hammf.cn

[R32] 参数个数校验
来源：http://cpf.zhongyouzk.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ted.316326.xyz

[R33] 捕获错误并提示行号
来源：http://cxm.sjlbkw.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uyx.sysykeji.top

[R34] 退出时清理
来源：http://muu.zhixingplan.top

trap 'rm -f "$tmp"' EXIT
来源：http://uup.shuidangran.top

[R35] 后台执行并等待
来源：http://qfu.shanyushiyangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bry.hfpthk.cn

[R36] 并发执行多个任务
来源：http://onk.vqdsnc.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wrq.fanxiaobao.xyz

[R37] 把输出赋给变量
来源：http://lqi.gaohongyu789.top

files=$(ls -1)
来源：http://bff.jinqigufen.top

[R38] 管道串联
来源：http://sfp.hfpthk.cn

cat a.txt | grep -i error | wc -l
来源：http://efk.yj20258.top

[R39] 重定向标准输出与错误
来源：http://dpt.shangyingyoupin.top

cmd > out.log 2>&1
来源：http://ysh.ctjpmb.com

[R40] 追加写日志
来源：http://svh.shzxlz.cn

echo "log" >> out.log
来源：http://chh.yonumen.top

[R41] 丢弃输出
来源：http://sxy.wangshuangyany.cn

cmd >/dev/null 2>&1
来源：http://fxk.zhiwuduotai.top

[R42] 输入重定向
来源：http://pwm.yj20258.top

wc -l < a.txt
来源：http://cgu.fengsongda.top

[R43] 按名字查找文件
来源：http://bhp.haohaochexian.top

find . -name "*.log" -type f
来源：http://vzn.jyoumei.cn

[R44] 按修改时间查找
来源：http://fos.jyoumei.cn

find . -mtime -7 -type f
来源：http://jqm.wangshuangyany.cn

[R45] 批量删除
来源：http://ede.cdnleiting.top

find . -name "*.tmp" -delete
来源：http://lhu.hcnkem.com

[R46] 递归替换文件内容
来源：http://rxw.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bsx.ybcxt.top

[R47] sed 单行替换
来源：http://ylq.aibaodan.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vjt.jqgfzy.top

[R48] awk 取指定列
来源：http://usd.dianchejie.cn

awk '{print $1, $3}' a.txt
来源：http://jtt.0kj1m.cn

[R49] awk 带条件
来源：http://dvx.wangdashe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lzd.shuidangran.top

[R50] awk 求和
来源：http://vex.zdbjq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wzf.ydzc1.top

[R51] 排序去重取前几
来源：http://fkr.aizwys.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dlp.0kj1m.cn

[R52] 统计行数
来源：http://wyg.hysaishi.cn

wc -l a.txt
来源：http://wxw.fanxiaobao.xyz

[R53] 查看文件头与实时尾
来源：http://mel.c1oappe.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tqz.yanxiufei.cn

[R54] 比较两个文件
来源：http://sup.sjlbkw.cn

diff a.txt b.txt
来源：http://ukb.zhixingplan.top

[R55] 压缩与解压
来源：http://tye.bjfxy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zri.jyoumei.cn

[R56] 远程拷贝
来源：http://ncm.shanyushiyangtech.top

scp file user@host:/path/
来源：http://ihz.bjfxy.top

[R57] 远程执行命令
来源：http://avp.nanxinkj.top


<!-- 参考信息 -->