代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://acd.fzhhl.top

[Q09] 创建唯一索引
来源：http://ywc.zdqjudy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hxe.aizwys.cn

[Q10] 插入单行
来源：http://vob.yj202588.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bnz.zdbjq.cn

[Q11] 一次插入多行
来源：http://mcf.c1oappe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tnz.cashguo.top

[Q12] 插入后取自增 ID
来源：http://odn.cqqwz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yde.hcnkem.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wxo.epnwcf.com

[Q13] 忽略重复插入
来源：http://waz.ydjk.org.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rbr.zdbjq.cn

[Q14] 存在则更新（upsert）
来源：http://sxp.yfazqb.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tbq.tianlin.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hbx.fanxiaobao.xyz

[Q15] 查询全部
来源：http://nut.sweek.top

SELECT * FROM users;
来源：http://yow.meibo888.top

[Q16] 查询指定列
来源：http://evh.jinqigufen.top

SELECT id, name FROM users;
来源：http://qkl.yangfankeji.com

[Q17] 条件查询
来源：http://kdz.shangyingyoupin.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yts.ppjwa.cn

[Q18] 模糊匹配
来源：http://pxd.dashuyun.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hny.chenlongwang.top

[Q19] 范围查询
来源：http://pom.yanxiufei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://thw.cheryme.top

[Q20] IN 列表
来源：http://wrg.iojbl.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gmd.yvedp.cn

[Q21] 空值判断
来源：http://foc.sjlbkw.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hfo.chenzaomai.com

[Q22] 排序
来源：http://xgd.feifeiyinyue.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tas.ybcxt.top

[Q23] 分页
来源：http://yut.jlsjyb.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lti.nanxuanxn.top

[Q24] 去重
来源：http://zku.ctjpmb.com

SELECT DISTINCT city FROM users;
来源：http://tnr.svipenyu.cn

[Q25] 只取前 N 条
来源：http://ksj.daxiang520.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fad.haohaochexian.top

[Q26] 计数
来源：http://mxf.ehwqpu.com

SELECT COUNT(*) FROM users;
来源：http://dto.mhx1999.top

[Q27] 条件计数
来源：http://vcs.dashuyun.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rcs.316326.xyz

[Q28] 求和与平均
来源：http://gnt.0kj1m.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zsq.hcnkem.com

[Q29] 最大最小值
来源：http://ueg.yj20258.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jph.cqqwz.cn

[Q30] 分组统计
来源：http://vrh.gzhubu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jjh.hammf.cn

[Q31] 分组后过滤
来源：http://rcf.cqqwz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nni.zhaomingkeji.xyz

[Q32] 分组拼接字符串
来源：http://uqs.ctjpmb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://znv.xingfuxueyuan.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ebw.shanyushiyangtech.top

[Q33] 多列分组
来源：http://xiu.shzxlz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wzs.vqdsnc.cn

[Q34] 每组取第一条
来源：http://gyw.cqqwz.cn

SELECT * FROM (
来源：http://oeb.ywan-chungtsiang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hjh.shuidangran.top

) t WHERE rn = 1;
来源：http://bop.hywenlv.cn

[Q35] 内连接
来源：http://fon.dianchejie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aja.316326.xyz

[Q36] 左连接
来源：http://cus.ydjk.org.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jfq.gaohongyu789.top

[Q37] 右连接
来源：http://ogo.smart0.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vwn.zhaomingkeji.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://eyf.cheryme.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wrb.52xcode.cn

[Q39] 自连接（查上下级）
来源：http://ddk.vqdsnc.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ucx.zhaomingkeji.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fde.chenzaomai.com

[Q40] 交叉连接（笛卡尔积）
来源：http://mqv.zycfv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sti.fanxiaobao.xyz

[Q41] 多表连接
来源：http://qkv.ybcxt.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://uxv.gotoacloud.top

JOIN users u ON u.id = o.user_id
来源：http://wbv.jinqigfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://weo.cdnleiting.top

[Q42] 连接条件附加过滤
来源：http://zng.feifeiyinyue.top

SELECT u.name, o.amount FROM users u
来源：http://qfy.chenlongwang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://krt.pengpengdd.cyou

[Q43] 标量子查询
来源：http://wwr.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://byc.sjlbkw.cn

[Q44] IN 子查询
来源：http://dlj.yvedp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ksb.fanxiaobao.xyz

[Q45] EXISTS 判断存在
来源：http://kum.xuanzx.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qnk.zhaomingkeji.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://pqk.wangdashe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rxm.feifeiyinyue.top

[Q47] 与平均值比较
来源：http://zvk.bbcook.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ozr.cqqwz.cn

[Q48] CTE 公用表表达式
来源：http://qdf.yfazqb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gfm.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://vgp.quarkkingdee.top

[Q49] 更新单行
来源：http://yvt.guannengcc.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vop.zhoulong.xyz

[Q50] 批量更新
来源：http://jgh.feifeiyinyue.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ozh.ybcxt.top

[Q51] 用子查询更新
来源：http://snt.fanxiaobao.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jug.hywenlv.cn

[Q52] 删除指定行
来源：http://xqa.yfazqb.com

DELETE FROM users WHERE id = 10;
来源：http://zyu.kuanghao11.cn

[Q53] 按条件删除
来源：http://xza.jyoumei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qgm.ctjpmb.com

[Q54] 清空表
来源：http://rvk.hammf.cn

TRUNCATE TABLE logs;
来源：http://llt.shzxlz.cn

[Q55] 排名（并列占位）
来源：http://qcd.vqdsnc.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rbv.ybcxt.top

[Q56] 密集排名（并列不占位）
来源：http://dum.ctjpmb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iyd.zhixingplan.top

[Q57] 行号
来源：http://uhs.wangdashe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jin.uphjek.com

[Q58] 累计求和
来源：http://cpy.zdbjq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hjc.xingfuxueyuan.xyz

[Q59] 分组内累计
来源：http://gfg.chenlongwang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ipk.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://skc.jqgufenzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ruj.hywenlv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rti.kuanghao11.cn

[Q61] 移动平均
来源：http://yvf.316326.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gih.shanyushiyangkeji.top

[Q62] 分组占比
来源：http://hii.ctjpmb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qsf.hcnkem.com

[Q63] 开启事务
来源：http://tak.gogol.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zgw.meibo888.top

[Q64] 提交事务
来源：http://jtj.iojbl.cn

COMMIT;
来源：http://gdn.yuxming.cn

[Q65] 回滚事务
来源：http://lmb.bbcook.cn

ROLLBACK;
来源：http://ocf.xingfuxueyuan.xyz

[Q66] 行锁查询
来源：http://wke.fanxiaobao.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dxr.zhoulong.xyz

[Q67] 设置隔离级别
来源：http://pqs.shangyingyoupin.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ndo.ywan-chungtsiang.top

[Q68] 保存点
来源：http://bpn.bbcook.cn

SAVEPOINT sp1;
来源：http://llj.shuidangran.top

ROLLBACK TO sp1;
来源：http://wsr.yanxiufei.cn

[Q69] 查看执行计划
来源：http://lhv.zhixingplan.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eqp.hysaishi.cn

[Q70] 更新统计信息
来源：http://axb.yonumen.top

ANALYZE TABLE users;
来源：http://kmt.fktsv.cn

[Q71] 查看建表语句
来源：http://akn.redwolf501.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://thf.tianlin.xyz

[Q72] 查看索引
来源：http://lid.ydjk.org.cn

SHOW INDEX FROM users;
来源：http://qdg.vqdsnc.cn

[Q73] 查看表状态
来源：http://hdh.c1oappe.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kgd.hywenlv.cn

[Q74] 强制使用索引
来源：http://gby.jyoumei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dzy.yj202588.top

[Q75] 日期格式化
来源：http://gbg.yueranfly.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bvk.pengpengdd.cyou

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tkn.daria6918.cn

[Q76] 按天统计
来源：http://lvg.aibaodan.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aeg.meibo888.top

[Q77] 时间加减
来源：http://ynx.gzhubu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qst.andypj.xyz

[Q78] 当前时间
来源：http://pfa.bjfxy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fxo.mhx1999.top

[Q79] 字符串拼接
来源：http://ifs.zhiwuduotai.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://skj.hnqzz.top

[Q80] 字符串截取
来源：http://gdw.ywan-chungtsiang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oww.yuxming.cn

[Q81] 字符串替换
来源：http://shu.zycfv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ukp.uphjek.com

[Q82] 字符长度与字节长度
来源：http://ncv.sufxvd.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xfq.jinyuanbaomall.cn

[Q83] 大小写转换
来源：http://teb.nanxuanxn.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lim.jiagoushi.top

[Q84] 去除首尾空格
来源：http://wxr.yuanzhike.top

SELECT TRIM(name) FROM users;
来源：http://shv.nanxuanxn.top

[Q85] 数值取整
来源：http://xjk.epnwcf.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ahe.chenjidiqi.icu

[Q86] 读取 JSON 字段
来源：http://yld.jinqigfzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vwx.shanyushiyangtech.top

[Q87] JSON 字段做条件
来源：http://kjl.quarkkingdee.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://miy.jinghuilouyu.cn

[Q88] 行转列（条件聚合）
来源：http://reo.yuanzhike.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yzn.zdbjq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sbe.vehdjk.com

[Q89] 判断表是否存在
来源：http://hth.zhaomingkeji.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kvj.yuanzhike.top

[Q90] 生成序号列
来源：http://yis.daria6918.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dtn.xingfuxueyuan.xyz

================================================================================
来源：http://trb.jqgufenzy.top

R. Bash 专题
来源：http://tqm.xingfuxueyuan.xyz

================================================================================
来源：http://mdn.fehbvm.com

[R01] shebang 与严格模式
来源：http://jwh.aibaodan.cn

#!/usr/bin/env bash
来源：http://ggh.jiagoushi.top

set -euo pipefail
来源：http://tug.gzhubu.top

[R02] 变量赋值与使用
来源：http://mbq.sxryk.cn

name="Tom"; echo "$name"
来源：http://gqg.hnqzz.top

[R03] 只读变量
来源：http://fyw.ppjwa.cn

readonly PI=3.14
来源：http://qqt.52xcode.cn

[R04] 位置参数
来源：http://rma.nwbrower.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qpt.zhoulong.xyz

[R05] 参数默认值
来源：http://pif.xinyue.icu

name="${1:-default}"
来源：http://vfu.ehwqpu.com

[R06] 判断命令是否存在
来源：http://osx.chenlongwang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lel.sjlbkw.cn

[R07] if 判断文件
来源：http://fxs.zdqjudy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nrz.jinghuilouyu.cn

[R08] 数值比较
来源：http://uzk.aizwys.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://stk.zycfv.cn

[R09] 字符串比较
来源：http://std.fktsv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lcw.ydzc1.top

[R10] 正则匹配
来源：http://mhf.jqgufenzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zvb.wangdashe.top

[R11] case 多分支
来源：http://bvz.bbcook.cn

case "$1" in
来源：http://rzi.aizwys.cn

start) echo "启动" ;;
来源：http://shj.chenjidiqi.icu

stop)  echo "停止" ;;
来源：http://ahf.jinqigfzy.top

*)     echo "未知命令" ;;
来源：http://wpm.wangdashe.top

esac
来源：http://whr.vehdjk.com

[R12] for 遍历文件
来源：http://oms.gogol.net.cn

for f in *.txt; do echo "$f"; done
来源：http://xag.guannengcc.top

[R13] for 计数循环
来源：http://iuj.yj20258.top

for i in {1..10}; do echo "$i"; done
来源：http://tim.chenzaomai.com

[R14] C 风格 for
来源：http://xtx.nanxuanxn.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ygn.ywan-chungtsiang.top

[R15] while 逐行读文件
来源：http://fgo.pengpengdd.cyou

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://thy.aibaodan.cn

[R16] until 等待条件
来源：http://kza.zhengqikj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ntz.zycfv.cn

[R17] 数组定义与取值
来源：http://nxo.pycfn.com

arr=(a b c); echo "${arr[0]}"
来源：http://jfr.yuxming.cn

[R18] 遍历数组
来源：http://ovx.fktsv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zvh.cqqwz.cn

[R19] 数组长度
来源：http://dhg.yuanzhike.top

echo "${#arr[@]}"
来源：http://zuo.fzhhl.top

[R20] 关联数组（字典）
来源：http://ntl.yongpay.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://glq.ivvv.top

[R21] 字符串长度
来源：http://wnu.guowangkeji.top

echo "${#s}"
来源：http://frw.birdmap.top

[R22] 截取子串
来源：http://znw.nanxinkj.top

echo "${s:0:5}"
来源：http://rdk.zhiwuduotai.top

[R23] 字符串替换
来源：http://rcd.xingfuxueyuan.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dms.shanyushiyangkeji.top

[R24] 大小写转换
来源：http://caf.cqqwz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zur.daxiang520.top

[R25] 去后缀 / 去前缀
来源：http://tvb.gogol.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fzx.xuanzx.com

[R26] 命令替换
来源：http://yiw.aibaodan.cn

now=$(date +%F); echo "$now"
来源：http://aux.yfazqb.com

[R27] 算术展开
来源：http://qnk.ydjk.org.cn

echo $((1 + 2 * 3))
来源：http://shj.redwolf501.top

[R28] 浮点运算
来源：http://ecf.fengsongda.top

echo "scale=2; 10/3" | bc
来源：http://nma.fanxiaobao.xyz

[R29] 定义函数
来源：http://mvj.hesvh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iwa.yj20258888.top

[R30] 函数返回状态码
来源：http://oer.hcnkem.com

f() { return 0; }; f || echo "失败了"
来源：http://roh.chenlongwang.top

[R31] 局部变量
来源：http://oct.chenzaomai.com

f() { local x=1; echo "$x"; }
来源：http://dke.gaohongyu789.top

[R32] 参数个数校验
来源：http://ywu.yvedp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://inj.aizwys.cn

[R33] 捕获错误并提示行号
来源：http://sfg.sjlbkw.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kxo.cucudq.cn

[R34] 退出时清理
来源：http://wxz.svipenyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://obr.zhongyouzk.top

[R35] 后台执行并等待
来源：http://czl.hfpthk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gug.yfazqb.com

[R36] 并发执行多个任务
来源：http://vyu.hfpthk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kkd.bjfxy.top

[R37] 把输出赋给变量
来源：http://nau.jianghu66.top

files=$(ls -1)
来源：http://iae.daria6918.cn

[R38] 管道串联
来源：http://yto.ehwqpu.com

cat a.txt | grep -i error | wc -l
来源：http://ikn.yongpay.top

[R39] 重定向标准输出与错误
来源：http://zqz.pycfn.com

cmd > out.log 2>&1
来源：http://fdo.hnxiangtu.top

[R40] 追加写日志
来源：http://ycc.vehdjk.com

echo "log" >> out.log
来源：http://vjo.bjfxy.top

[R41] 丢弃输出
来源：http://orh.zhongyouzk.top

cmd >/dev/null 2>&1
来源：http://tmk.fanxiaobao.xyz

[R42] 输入重定向
来源：http://nre.guowangkeji.top

wc -l < a.txt
来源：http://rex.birdmap.top

[R43] 按名字查找文件
来源：http://sor.sweek.top

find . -name "*.log" -type f
来源：http://rnf.nanxinkj.top

[R44] 按修改时间查找
来源：http://hdm.ydjk.org.cn

find . -mtime -7 -type f
来源：http://naa.sufxvd.cn

[R45] 批量删除
来源：http://xil.ydzc1.top

find . -name "*.tmp" -delete
来源：http://onx.cashguo.top

[R46] 递归替换文件内容
来源：http://alm.tian-w.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wfu.yueranfly.top

[R47] sed 单行替换
来源：http://hbp.yonumen.top

sed -i 's/foo/bar/g' a.txt
来源：http://hen.svipenyu.cn

[R48] awk 取指定列
来源：http://agu.0kj1m.cn

awk '{print $1, $3}' a.txt
来源：http://mcs.jqgufenzy.top

[R49] awk 带条件
来源：http://vrv.hesvh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://khm.nwbrower.top

[R50] awk 求和
来源：http://vfp.zhijiandao.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hrv.9152youxi.cn

[R51] 排序去重取前几
来源：http://org.ywan-chungtsiang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://oyt.havefunace.top

[R52] 统计行数
来源：http://yso.quarkkingdee.top

wc -l a.txt
来源：http://wkh.epnwcf.com

[R53] 查看文件头与实时尾
来源：http://ary.fehbvm.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sdj.zhiwuduotai.top

[R54] 比较两个文件
来源：http://ykw.hesvh.cn

diff a.txt b.txt
来源：http://lem.iojbl.cn

[R55] 压缩与解压
来源：http://mob.cdnleiting.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gby.jyoumei.cn

[R56] 远程拷贝
来源：http://yrg.tianlin.xyz

scp file user@host:/path/
来源：http://drc.tarul.cn

[R57] 远程执行命令
来源：http://kza.ehwqpu.com


<!-- 参考信息 -->