代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://twq.jinyuanbaomall.cn

[Q09] 创建唯一索引
来源：http://iyg.chenlongwang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yal.yfazqb.com

[Q10] 插入单行
来源：http://cni.0kj1m.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cud.shzxlz.cn

[Q11] 一次插入多行
来源：http://han.jianghu66.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zzg.cashguo.top

[Q12] 插入后取自增 ID
来源：http://bsq.svipenyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mft.aizwys.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pfy.iojbl.cn

[Q13] 忽略重复插入
来源：http://ick.xinyue.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vvh.sjlbkw.cn

[Q14] 存在则更新（upsert）
来源：http://exg.hfpthk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://owi.xylfe.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tag.jyoumei.cn

[Q15] 查询全部
来源：http://pgw.52xcode.cn

SELECT * FROM users;
来源：http://jxi.pengpengdd.cyou

[Q16] 查询指定列
来源：http://dkd.yj20258888.top

SELECT id, name FROM users;
来源：http://qnr.jinqigufen.top

[Q17] 条件查询
来源：http://tvv.sysykeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://soe.chenjidiqi.icu

[Q18] 模糊匹配
来源：http://znq.316326.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yyr.0kj1m.cn

[Q19] 范围查询
来源：http://oib.xylfe.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ujq.hnxiangtu.top

[Q20] IN 列表
来源：http://tcb.xinyue.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pha.ydjk.org.cn

[Q21] 空值判断
来源：http://zpz.chenlongwang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://esc.52xcode.cn

[Q22] 排序
来源：http://anv.fehbvm.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://apv.dianchejie.cn

[Q23] 分页
来源：http://vrv.hongshengwenyu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rig.316326.xyz

[Q24] 去重
来源：http://edr.zhiwuduotai.top

SELECT DISTINCT city FROM users;
来源：http://cyn.zhoulong.xyz

[Q25] 只取前 N 条
来源：http://brs.cqqwz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kdz.hongshengwenyu.top

[Q26] 计数
来源：http://slj.zdbjq.cn

SELECT COUNT(*) FROM users;
来源：http://cjo.shanyushiyangtech.top

[Q27] 条件计数
来源：http://xnw.andypj.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bxm.xuanzx.com

[Q28] 求和与平均
来源：http://xdx.gzhubu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pxh.feifeiyinyue.top

[Q29] 最大最小值
来源：http://dsz.sweek.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ird.ctjpmb.com

[Q30] 分组统计
来源：http://udl.nanxuanxn.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yos.yonumen.top

[Q31] 分组后过滤
来源：http://ipk.jiagoushi.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zct.zhijiandao.cn

[Q32] 分组拼接字符串
来源：http://mme.jiagoushi.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cal.0kj1m.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fkd.guowangkeji.top

[Q33] 多列分组
来源：http://kso.sufxvd.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yoc.gaohongyu789.top

[Q34] 每组取第一条
来源：http://nlg.tarul.cn

SELECT * FROM (
来源：http://kfb.gaohongyu789.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sal.zhoulong.xyz

) t WHERE rn = 1;
来源：http://eia.epnwcf.com

[Q35] 内连接
来源：http://wpy.cqqwz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kuy.smart0.xyz

[Q36] 左连接
来源：http://pue.svipenyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hny.cheryme.top

[Q37] 右连接
来源：http://sxr.feifeiyinyue.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://biz.hysaishi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jnc.guowangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ool.zhongyouzk.top

[Q39] 自连接（查上下级）
来源：http://ins.chenzaomai.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://kmk.yvedp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sum.cashguo.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pld.daria6918.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://inw.zhiwuduotai.top

[Q41] 多表连接
来源：http://tzi.nanxinkj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fgc.yueranfly.top

JOIN users u ON u.id = o.user_id
来源：http://vis.jqgfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://gel.cucudq.cn

[Q42] 连接条件附加过滤
来源：http://fjo.yvedp.cn

SELECT u.name, o.amount FROM users u
来源：http://puj.wangdashe.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hqx.c1oappe.top

[Q43] 标量子查询
来源：http://qns.zycfv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gyk.zhongyouzk.top

[Q44] IN 子查询
来源：http://bpt.xylfe.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gkj.ybcxt.top

[Q45] EXISTS 判断存在
来源：http://smk.yanxiufei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lkp.kuanghao11.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kqw.aibaodan.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jdb.jinyuanbaomall.cn

[Q47] 与平均值比较
来源：http://pjo.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ylj.xylfe.cn

[Q48] CTE 公用表表达式
来源：http://cgk.aizwys.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mdc.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://jzg.chenzaomai.com

[Q49] 更新单行
来源：http://zux.yvedp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mtk.yueranfly.top

[Q50] 批量更新
来源：http://snd.vehdjk.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ttl.jinyuanbaomall.cn

[Q51] 用子查询更新
来源：http://pyd.andypj.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kuw.ywan-chungtsiang.top

[Q52] 删除指定行
来源：http://cfo.tanke756.top

DELETE FROM users WHERE id = 10;
来源：http://ojp.fengsongda.top

[Q53] 按条件删除
来源：http://qvn.chenjidiqi.icu

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cpo.yueranfly.top

[Q54] 清空表
来源：http://fkn.jinqigfzy.top

TRUNCATE TABLE logs;
来源：http://vcz.daria6918.cn

[Q55] 排名（并列占位）
来源：http://vej.shzxlz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iie.yj202588.top

[Q56] 密集排名（并列不占位）
来源：http://dcc.zhijiandao.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zsd.zhijiandao.cn

[Q57] 行号
来源：http://tfj.yuanzhike.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tjg.jinghuilouyu.cn

[Q58] 累计求和
来源：http://myj.shangyingyoupin.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://djt.andypj.xyz

[Q59] 分组内累计
来源：http://cai.shanyushiyangtech.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nip.ywan-chungtsiang.top

[Q60] 取上一行 / 下一行
来源：http://ofi.cucudq.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aiv.0kj1m.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kcd.zhixingplan.top

[Q61] 移动平均
来源：http://twx.ctjpmb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ekd.dianchejie.cn

[Q62] 分组占比
来源：http://cgz.havefunace.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kuz.jinghuilouyu.cn

[Q63] 开启事务
来源：http://igr.pengpengdd.cyou

START TRANSACTION;                -- 或 BEGIN
来源：http://ckb.yonumen.top

[Q64] 提交事务
来源：http://dqg.shuidangran.top

COMMIT;
来源：http://kro.daxiang520.top

[Q65] 回滚事务
来源：http://lut.fktsv.cn

ROLLBACK;
来源：http://mxb.dashuyun.cn

[Q66] 行锁查询
来源：http://ghr.zdqjudy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kdi.fanxiaobao.xyz

[Q67] 设置隔离级别
来源：http://tnv.zhiwuduotai.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pel.hfpthk.cn

[Q68] 保存点
来源：http://esp.fzhhl.top

SAVEPOINT sp1;
来源：http://nce.xinyue.icu

ROLLBACK TO sp1;
来源：http://yyh.cqqwz.cn

[Q69] 查看执行计划
来源：http://bay.tianlin.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gzo.nanxuanxn.top

[Q70] 更新统计信息
来源：http://zhw.fzhhl.top

ANALYZE TABLE users;
来源：http://jsn.guowangkeji.top

[Q71] 查看建表语句
来源：http://dko.yangfankeji.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hbp.fktsv.cn

[Q72] 查看索引
来源：http://dpu.fzhhl.top

SHOW INDEX FROM users;
来源：http://mri.jyoumei.cn

[Q73] 查看表状态
来源：http://jmx.tianlin.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://uxl.uphjek.com

[Q74] 强制使用索引
来源：http://psa.epnwcf.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sqv.fengsongda.top

[Q75] 日期格式化
来源：http://orf.daria6918.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pfu.fehbvm.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qrj.zhaomingkeji.xyz

[Q76] 按天统计
来源：http://tys.yongpay.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yyp.yonumen.top

[Q77] 时间加减
来源：http://ezh.ctjpmb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uox.hammf.cn

[Q78] 当前时间
来源：http://rlg.xingfuxueyuan.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://csx.hnxiangtu.top

[Q79] 字符串拼接
来源：http://tgx.daxiang520.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://plf.guowangkeji.top

[Q80] 字符串截取
来源：http://ngy.yongpay.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://umn.hysaishi.cn

[Q81] 字符串替换
来源：http://mew.bjfxy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kdq.chenzaomai.com

[Q82] 字符长度与字节长度
来源：http://ymj.feifeiyinyue.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xgr.hfpthk.cn

[Q83] 大小写转换
来源：http://ilo.0kj1m.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://diz.tianlin.xyz

[Q84] 去除首尾空格
来源：http://gij.epnwcf.com

SELECT TRIM(name) FROM users;
来源：http://aho.ehwqpu.com

[Q85] 数值取整
来源：http://bec.shzxlz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ixu.tanke756.top

[Q86] 读取 JSON 字段
来源：http://gin.bjfxy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ytj.zycfv.cn

[Q87] JSON 字段做条件
来源：http://llh.fzhhl.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yca.jlsjyb.cn

[Q88] 行转列（条件聚合）
来源：http://vvj.shangyingyoupin.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ypv.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://huk.xingfuxueyuan.xyz

[Q89] 判断表是否存在
来源：http://xab.0kj1m.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rox.feifeiyinyue.top

[Q90] 生成序号列
来源：http://qpi.ehwqpu.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ump.fanxiaobao.xyz

================================================================================
来源：http://gye.ehwqpu.com

R. Bash 专题
来源：http://xks.jinghuilouyu.cn

================================================================================
来源：http://lvq.jqgufenzy.top

[R01] shebang 与严格模式
来源：http://lfq.shangyingyoupin.top

#!/usr/bin/env bash
来源：http://yhl.ehwqpu.com

set -euo pipefail
来源：http://mpl.havefunace.top

[R02] 变量赋值与使用
来源：http://ukz.ehwqpu.com

name="Tom"; echo "$name"
来源：http://nga.fzhhl.top

[R03] 只读变量
来源：http://dzq.yangfankeji.com

readonly PI=3.14
来源：http://pfx.hywenlv.cn

[R04] 位置参数
来源：http://abk.jinqigfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pdr.chenlongwang.top

[R05] 参数默认值
来源：http://wom.hammf.cn

name="${1:-default}"
来源：http://pke.ehwqpu.com

[R06] 判断命令是否存在
来源：http://eew.ppjwa.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eef.guannengcc.top

[R07] if 判断文件
来源：http://tir.cqqwz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fqk.gotoacloud.top

[R08] 数值比较
来源：http://toy.jinqigufen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cnv.guannengcc.top

[R09] 字符串比较
来源：http://uxq.hnqzz.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qks.yfazqb.com

[R10] 正则匹配
来源：http://pkq.jinqigfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cof.ywan-chungtsiang.top

[R11] case 多分支
来源：http://qph.guowangkeji.top

case "$1" in
来源：http://dzw.tanke756.top

start) echo "启动" ;;
来源：http://and.jinqigufen.top

stop)  echo "停止" ;;
来源：http://zby.uphjek.com

*)     echo "未知命令" ;;
来源：http://bjt.ydjk.org.cn

esac
来源：http://ffm.gotoacloud.top

[R12] for 遍历文件
来源：http://jpt.ehwqpu.com

for f in *.txt; do echo "$f"; done
来源：http://vzd.wangshuangyany.cn

[R13] for 计数循环
来源：http://yov.ydzc1.top

for i in {1..10}; do echo "$i"; done
来源：http://niy.yj20258.top

[R14] C 风格 for
来源：http://kdc.jyoumei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bon.sjlbkw.cn

[R15] while 逐行读文件
来源：http://wxu.sysykeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ppx.ybcxt.top

[R16] until 等待条件
来源：http://ynl.hongshengwenyu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://trg.sysykeji.top

[R17] 数组定义与取值
来源：http://wqy.wangshuangyany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zqm.pengpengdd.cyou

[R18] 遍历数组
来源：http://wxg.mhx1999.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uwf.yj20258888.top

[R19] 数组长度
来源：http://mhx.fktsv.cn

echo "${#arr[@]}"
来源：http://tmz.ivvv.top

[R20] 关联数组（字典）
来源：http://xel.yuanzhike.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://txf.ydzc1.top

[R21] 字符串长度
来源：http://wvk.jinqigfzy.top

echo "${#s}"
来源：http://ekj.jianghu66.top

[R22] 截取子串
来源：http://fyi.sysykeji.top

echo "${s:0:5}"
来源：http://eqk.tarul.cn

[R23] 字符串替换
来源：http://bhe.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jbk.sysykeji.top

[R24] 大小写转换
来源：http://tyb.nwbrower.top

echo "${s^^}"; echo "${s,,}"
来源：http://wft.daxiang520.top

[R25] 去后缀 / 去前缀
来源：http://ftj.fanxiaobao.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://wjk.gotoacloud.top

[R26] 命令替换
来源：http://gmf.daxiang520.top

now=$(date +%F); echo "$now"
来源：http://xgw.aibaodan.cn

[R27] 算术展开
来源：http://awo.sxryk.cn

echo $((1 + 2 * 3))
来源：http://lbk.c1oappe.top

[R28] 浮点运算
来源：http://ncg.shanyushiyangkeji.top

echo "scale=2; 10/3" | bc
来源：http://lht.yj202588.top

[R29] 定义函数
来源：http://cvy.pycfn.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cao.shuidangran.top

[R30] 函数返回状态码
来源：http://mrl.meibo888.top

f() { return 0; }; f || echo "失败了"
来源：http://wmc.jiagoushi.top

[R31] 局部变量
来源：http://uiv.dashuyun.cn

f() { local x=1; echo "$x"; }
来源：http://psd.ppjwa.cn

[R32] 参数个数校验
来源：http://gpp.feifeiyinyue.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://whg.cheryme.top

[R33] 捕获错误并提示行号
来源：http://xod.shzxlz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ion.jinqigfzy.top

[R34] 退出时清理
来源：http://kby.zhixingplan.top

trap 'rm -f "$tmp"' EXIT
来源：http://okq.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://ukm.cucudq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pxh.zdqjudy.top

[R36] 并发执行多个任务
来源：http://hye.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lia.zhijiandao.cn

[R37] 把输出赋给变量
来源：http://wcb.tarul.cn

files=$(ls -1)
来源：http://bjx.jinyuanbaomall.cn

[R38] 管道串联
来源：http://pfd.yueranfly.top

cat a.txt | grep -i error | wc -l
来源：http://guj.tian-w.cn

[R39] 重定向标准输出与错误
来源：http://vgt.jqgufenzy.top

cmd > out.log 2>&1
来源：http://eln.ctjpmb.com

[R40] 追加写日志
来源：http://twp.gaohongyu789.top

echo "log" >> out.log
来源：http://pkz.shzxlz.cn

[R41] 丢弃输出
来源：http://arj.yueranfly.top

cmd >/dev/null 2>&1
来源：http://qnv.aibaodan.cn

[R42] 输入重定向
来源：http://ari.jlsjyb.cn

wc -l < a.txt
来源：http://zqm.smart0.xyz

[R43] 按名字查找文件
来源：http://myz.xuanzx.com

find . -name "*.log" -type f
来源：http://cwu.xylfe.cn

[R44] 按修改时间查找
来源：http://auk.gaohongyu789.top

find . -mtime -7 -type f
来源：http://fnm.yueranfly.top

[R45] 批量删除
来源：http://vmq.tianlin.xyz

find . -name "*.tmp" -delete
来源：http://hom.yuxming.cn

[R46] 递归替换文件内容
来源：http://aad.sjlbkw.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://txp.jyoumei.cn

[R47] sed 单行替换
来源：http://tyk.birdmap.top

sed -i 's/foo/bar/g' a.txt
来源：http://jno.jinghuilouyu.cn

[R48] awk 取指定列
来源：http://ptr.chenjidiqi.icu

awk '{print $1, $3}' a.txt
来源：http://xwp.hysaishi.cn

[R49] awk 带条件
来源：http://uas.birdmap.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jev.fengsongda.top

[R50] awk 求和
来源：http://otn.yfazqb.com

awk '{s += $2} END {print s}' a.txt
来源：http://wgr.chenzaomai.com

[R51] 排序去重取前几
来源：http://zxr.cqqwz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vpc.meibo888.top

[R52] 统计行数
来源：http://wuy.daxiang520.top

wc -l a.txt
来源：http://apy.cashguo.top

[R53] 查看文件头与实时尾
来源：http://nvg.ybcxt.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ofz.smart0.xyz

[R54] 比较两个文件
来源：http://jmq.zdqjudy.top

diff a.txt b.txt
来源：http://ryt.hysaishi.cn

[R55] 压缩与解压
来源：http://sof.daria6918.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mra.gotoacloud.top

[R56] 远程拷贝
来源：http://mok.yfazqb.com

scp file user@host:/path/
来源：http://ikk.ehwqpu.com

[R57] 远程执行命令
来源：http://rju.mhx1999.top


<!-- 参考信息 -->