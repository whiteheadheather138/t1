代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://roi.havefunace.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rdq.yonumen.top

[Q13] 忽略重复插入
来源：http://ohs.yongpay.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dcv.cqqwz.cn

[Q14] 存在则更新（upsert）
来源：http://woi.chenlongwang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pvn.svipenyu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ihk.andypj.xyz

[Q15] 查询全部
来源：http://noc.hywenlv.cn

SELECT * FROM users;
来源：http://glv.cdnleiting.top

[Q16] 查询指定列
来源：http://axh.ctjpmb.com

SELECT id, name FROM users;
来源：http://feu.tianlin.xyz

[Q17] 条件查询
来源：http://xbp.zhijiandao.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eyj.ywan-chungtsiang.top

[Q18] 模糊匹配
来源：http://faa.gotoacloud.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://csx.yangfankeji.com

[Q19] 范围查询
来源：http://bjc.yfazqb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fpf.zhengqikj.top

[Q20] IN 列表
来源：http://eru.yuanzhike.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lrg.hnqzz.top

[Q21] 空值判断
来源：http://xeh.pycfn.com

SELECT * FROM users WHERE email IS NULL;
来源：http://xlv.gogol.net.cn

[Q22] 排序
来源：http://psr.kuanghao11.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zzk.zdbjq.cn

[Q23] 分页
来源：http://xyb.gogol.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fku.shanyushiyangkeji.top

[Q24] 去重
来源：http://wwv.shzxlz.cn

SELECT DISTINCT city FROM users;
来源：http://rvq.sjlbkw.cn

[Q25] 只取前 N 条
来源：http://asl.quarkkingdee.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yag.zhijiandao.cn

[Q26] 计数
来源：http://inu.gaohongyu789.top

SELECT COUNT(*) FROM users;
来源：http://utx.yuanzhike.top

[Q27] 条件计数
来源：http://ovf.vqdsnc.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rnu.jiagoushi.top

[Q28] 求和与平均
来源：http://xaw.guannengcc.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pop.jlsjyb.cn

[Q29] 最大最小值
来源：http://fmt.ywan-chungtsiang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://eua.redwolf501.top

[Q30] 分组统计
来源：http://cky.yueranfly.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://opm.aibaodan.cn

[Q31] 分组后过滤
来源：http://yez.shanyushiyangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qop.bjfxy.top

[Q32] 分组拼接字符串
来源：http://guy.jyoumei.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ajw.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tix.ehwqpu.com

[Q33] 多列分组
来源：http://kun.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hpa.jinyuanbaomall.cn

[Q34] 每组取第一条
来源：http://bfz.chenjidiqi.icu

SELECT * FROM (
来源：http://mqq.epnwcf.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://aab.bbcook.cn

) t WHERE rn = 1;
来源：http://fbz.jiagoushi.top

[Q35] 内连接
来源：http://zed.svipenyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bok.hcnkem.com

[Q36] 左连接
来源：http://fwq.birdmap.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pyw.smart0.xyz

[Q37] 右连接
来源：http://isx.meibo888.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nzn.nanxuanxn.top

[Q38] 全外连接（PostgreSQL）
来源：http://eqb.sufxvd.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lak.bbcook.cn

[Q39] 自连接（查上下级）
来源：http://sol.nwbrower.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://cez.yonumen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wzm.xziqi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://svr.ehwqpu.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kdx.hysaishi.cn

[Q41] 多表连接
来源：http://qzd.yvedp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fse.smart0.xyz

JOIN users u ON u.id = o.user_id
来源：http://szl.pengpengdd.cyou

JOIN products p ON p.id = o.product_id;
来源：http://izt.cdnleiting.top

[Q42] 连接条件附加过滤
来源：http://scv.bjfxy.top

SELECT u.name, o.amount FROM users u
来源：http://vbg.shuidangran.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nku.ivvv.top

[Q43] 标量子查询
来源：http://lrb.sysykeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jhn.cqqwz.cn

[Q44] IN 子查询
来源：http://ncu.epnwcf.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ilr.sufxvd.cn

[Q45] EXISTS 判断存在
来源：http://pag.ppjwa.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jxm.shanyushiyangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://ysy.0kj1m.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ldm.jqgufenzy.top

[Q47] 与平均值比较
来源：http://fuc.ehwqpu.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mnr.chenlongwang.top

[Q48] CTE 公用表表达式
来源：http://inm.jinqigufen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pra.birdmap.top

SELECT * FROM t WHERE c > 5;
来源：http://ckl.52xcode.cn

[Q49] 更新单行
来源：http://evl.fehbvm.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bmd.epnwcf.com

[Q50] 批量更新
来源：http://lac.hcnkem.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mxr.cdnleiting.top

[Q51] 用子查询更新
来源：http://qal.yuxming.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pus.jiagoushi.top

[Q52] 删除指定行
来源：http://vvl.guannengcc.top

DELETE FROM users WHERE id = 10;
来源：http://esi.jyoumei.cn

[Q53] 按条件删除
来源：http://eot.snrcjt.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ymw.cucudq.cn

[Q54] 清空表
来源：http://pzu.vqdsnc.cn

TRUNCATE TABLE logs;
来源：http://blh.pycfn.com

[Q55] 排名（并列占位）
来源：http://lgr.shanyushiyangkeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mlg.jqgfzy.top

[Q56] 密集排名（并列不占位）
来源：http://uvs.gogol.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yvk.cqqwz.cn

[Q57] 行号
来源：http://cvj.c1oappe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jtj.andypj.xyz

[Q58] 累计求和
来源：http://hit.sysykeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gys.ydzc1.top

[Q59] 分组内累计
来源：http://loy.dianchejie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lha.pengpengdd.cyou

[Q60] 取上一行 / 下一行
来源：http://upy.9152youxi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nwn.gogol.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wws.yonumen.top

[Q61] 移动平均
来源：http://hja.shanyushiyangtech.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qqu.ehwqpu.com

[Q62] 分组占比
来源：http://kbx.jinqigufen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hbq.jinyuanbaomall.cn

[Q63] 开启事务
来源：http://doj.chenzaomai.com

START TRANSACTION;                -- 或 BEGIN
来源：http://wiz.epnwcf.com

[Q64] 提交事务
来源：http://pyo.zhongyouzk.top

COMMIT;
来源：http://zco.yvedp.cn

[Q65] 回滚事务
来源：http://oud.daxiang520.top

ROLLBACK;
来源：http://ule.sweek.top

[Q66] 行锁查询
来源：http://mzn.aizwys.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kfq.snrcjt.cn

[Q67] 设置隔离级别
来源：http://miu.tianlin.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://txd.daxiang520.top

[Q68] 保存点
来源：http://bfm.epnwcf.com

SAVEPOINT sp1;
来源：http://zvu.ydjk.org.cn

ROLLBACK TO sp1;
来源：http://fqi.guannengcc.top

[Q69] 查看执行计划
来源：http://nmf.zdqjudy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ssb.sjlbkw.cn

[Q70] 更新统计信息
来源：http://tqc.gogol.net.cn

ANALYZE TABLE users;
来源：http://nww.yonumen.top

[Q71] 查看建表语句
来源：http://cab.cashguo.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fcn.shangyingyoupin.top

[Q72] 查看索引
来源：http://cun.feifeiyinyue.top

SHOW INDEX FROM users;
来源：http://qjc.fehbvm.com

[Q73] 查看表状态
来源：http://fco.cqqwz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cpl.jinqigufen.top

[Q74] 强制使用索引
来源：http://tte.jinqigfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ekq.chenzaomai.com

[Q75] 日期格式化
来源：http://dyy.cheryme.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://efl.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pkw.c1oappe.top

[Q76] 按天统计
来源：http://jbj.chenzaomai.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jas.nwbrower.top

[Q77] 时间加减
来源：http://yup.hammf.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nps.yj20258.top

[Q78] 当前时间
来源：http://fuv.ywan-chungtsiang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nrs.jianghu66.top

[Q79] 字符串拼接
来源：http://vgm.shanyushiyangtech.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pir.cucudq.cn

[Q80] 字符串截取
来源：http://egl.yfazqb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ioy.jqgufenzy.top

[Q81] 字符串替换
来源：http://fby.aibaodan.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mnp.shanyushiyangtech.top

[Q82] 字符长度与字节长度
来源：http://bar.meibo888.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tir.yj202588.top

[Q83] 大小写转换
来源：http://jwy.ybcxt.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://djw.tianlin.xyz

[Q84] 去除首尾空格
来源：http://oar.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://jxa.pycfn.com

[Q85] 数值取整
来源：http://kno.shuidangran.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://idf.zhaomingkeji.xyz

[Q86] 读取 JSON 字段
来源：http://ugx.hcnkem.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://byn.aibaodan.cn

[Q87] JSON 字段做条件
来源：http://xsf.vqdsnc.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ccq.vehdjk.com

[Q88] 行转列（条件聚合）
来源：http://swt.cucudq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ugg.uphjek.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hhi.chenlongwang.top

[Q89] 判断表是否存在
来源：http://rna.feifeiyinyue.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sil.uphjek.com

[Q90] 生成序号列
来源：http://dfh.birdmap.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://owc.jiagoushi.top

================================================================================
来源：http://vcr.fanxiaobao.xyz

R. Bash 专题
来源：http://rmg.yfazqb.com

================================================================================
来源：http://wmo.yongpay.top

[R01] shebang 与严格模式
来源：http://vcd.birdmap.top

#!/usr/bin/env bash
来源：http://ali.jqgfzy.top

set -euo pipefail
来源：http://avx.jinyuanbaomall.cn

[R02] 变量赋值与使用
来源：http://wnu.birdmap.top

name="Tom"; echo "$name"
来源：http://bpv.ydjk.org.cn

[R03] 只读变量
来源：http://yhl.zdqjudy.top

readonly PI=3.14
来源：http://wpn.yongpay.top

[R04] 位置参数
来源：http://auv.c1oappe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jdl.yj20258888.top

[R05] 参数默认值
来源：http://euz.daxiang520.top

name="${1:-default}"
来源：http://vjm.zhongyouzk.top

[R06] 判断命令是否存在
来源：http://ajy.ppjwa.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://igp.yuanzhike.top

[R07] if 判断文件
来源：http://nea.yongpay.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ybb.ehwqpu.com

[R08] 数值比较
来源：http://hsg.bjfxy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nrc.jqgfzy.top

[R09] 字符串比较
来源：http://ugw.fanxiaobao.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://udc.ywan-chungtsiang.top

[R10] 正则匹配
来源：http://skx.zhixingplan.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wug.pengpengdd.cyou

[R11] case 多分支
来源：http://zcn.316326.xyz

case "$1" in
来源：http://zwo.yanxiufei.cn

start) echo "启动" ;;
来源：http://wdk.hcnkem.com

stop)  echo "停止" ;;
来源：http://txm.cdnleiting.top

*)     echo "未知命令" ;;
来源：http://uxr.redwolf501.top

esac
来源：http://nid.vqdsnc.cn

[R12] for 遍历文件
来源：http://xqe.ctjpmb.com

for f in *.txt; do echo "$f"; done
来源：http://uie.haohaochexian.top

[R13] for 计数循环
来源：http://txe.ivvv.top

for i in {1..10}; do echo "$i"; done
来源：http://eij.yj20258.top

[R14] C 风格 for
来源：http://xvc.shuidangran.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jca.jyoumei.cn

[R15] while 逐行读文件
来源：http://mta.yuanzhike.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://irj.yueranfly.top

[R16] until 等待条件
来源：http://ftn.fengsongda.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://aih.quarkkingdee.top

[R17] 数组定义与取值
来源：http://zsd.pycfn.com

arr=(a b c); echo "${arr[0]}"
来源：http://oxz.zhijiandao.cn

[R18] 遍历数组
来源：http://pec.ctjpmb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ipb.ehwqpu.com

[R19] 数组长度
来源：http://fmn.jyoumei.cn

echo "${#arr[@]}"
来源：http://rfh.aizwys.cn

[R20] 关联数组（字典）
来源：http://izj.0kj1m.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kvu.havefunace.top

[R21] 字符串长度
来源：http://qpp.shanyushiyangtech.top

echo "${#s}"
来源：http://zar.vehdjk.com

[R22] 截取子串
来源：http://obh.xuanzx.com

echo "${s:0:5}"
来源：http://eud.hnxiangtu.top

[R23] 字符串替换
来源：http://dgi.wangshuangyany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qee.fengsongda.top

[R24] 大小写转换
来源：http://luo.tianlin.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://yzh.gaohongyu789.top

[R25] 去后缀 / 去前缀
来源：http://ctf.zhijiandao.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bdm.c1oappe.top

[R26] 命令替换
来源：http://suv.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://eov.pengpengdd.cyou

[R27] 算术展开
来源：http://mji.chenlongwang.top

echo $((1 + 2 * 3))
来源：http://auq.fehbvm.com

[R28] 浮点运算
来源：http://xib.cashguo.top

echo "scale=2; 10/3" | bc
来源：http://iha.aizwys.cn

[R29] 定义函数
来源：http://tgr.haohaochexian.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xhi.hfpthk.cn

[R30] 函数返回状态码
来源：http://evj.tian-w.cn

f() { return 0; }; f || echo "失败了"
来源：http://oan.ydzc1.top

[R31] 局部变量
来源：http://wby.redwolf501.top

f() { local x=1; echo "$x"; }
来源：http://sci.dianchejie.cn

[R32] 参数个数校验
来源：http://fqg.sjlbkw.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ajo.tian-w.cn

[R33] 捕获错误并提示行号
来源：http://wbm.birdmap.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jne.fktsv.cn

[R34] 退出时清理
来源：http://pdc.yanxiufei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jbk.9152youxi.cn

[R35] 后台执行并等待
来源：http://byf.vqdsnc.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rrd.sysykeji.top

[R36] 并发执行多个任务
来源：http://lgd.yj202588.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vnt.sweek.top

[R37] 把输出赋给变量
来源：http://zrt.yj202588.top

files=$(ls -1)
来源：http://ijp.ehwqpu.com

[R38] 管道串联
来源：http://fsg.dashuyun.cn

cat a.txt | grep -i error | wc -l
来源：http://efa.uphjek.com

[R39] 重定向标准输出与错误
来源：http://nfn.cdnleiting.top

cmd > out.log 2>&1
来源：http://kac.guowangkeji.top

[R40] 追加写日志
来源：http://zxy.wangdashe.top

echo "log" >> out.log
来源：http://ejw.haohaochexian.top

[R41] 丢弃输出
来源：http://oni.mhx1999.top

cmd >/dev/null 2>&1
来源：http://uet.ydzc1.top

[R42] 输入重定向
来源：http://ovo.hcnkem.com

wc -l < a.txt
来源：http://gvt.guannengcc.top

[R43] 按名字查找文件
来源：http://wzd.gzhubu.top

find . -name "*.log" -type f
来源：http://rtz.zhaomingkeji.xyz

[R44] 按修改时间查找
来源：http://ffi.gaohongyu789.top

find . -mtime -7 -type f
来源：http://dyj.jinyuanbaomall.cn

[R45] 批量删除
来源：http://vav.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://ani.sysykeji.top

[R46] 递归替换文件内容
来源：http://enl.shuidangran.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wmu.fanxiaobao.xyz

[R47] sed 单行替换
来源：http://bnh.tanke756.top

sed -i 's/foo/bar/g' a.txt
来源：http://phv.dianchejie.cn

[R48] awk 取指定列
来源：http://fcp.yj202588.top

awk '{print $1, $3}' a.txt
来源：http://rdk.tianlin.xyz

[R49] awk 带条件
来源：http://jpn.haohaochexian.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qoz.haohaochexian.top

[R50] awk 求和
来源：http://wfu.jiagoushi.top

awk '{s += $2} END {print s}' a.txt
来源：http://xmr.shanyushiyangkeji.top

[R51] 排序去重取前几
来源：http://lan.guowangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ptr.zhiwuduotai.top

[R52] 统计行数
来源：http://vom.xinyue.icu

wc -l a.txt
来源：http://wha.pycfn.com

[R53] 查看文件头与实时尾
来源：http://ift.yuxming.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wtx.xuanzx.com

[R54] 比较两个文件
来源：http://wca.gogol.net.cn

diff a.txt b.txt
来源：http://mdt.cqqwz.cn

[R55] 压缩与解压
来源：http://jkc.jiagoushi.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://upe.chenlongwang.top

[R56] 远程拷贝
来源：http://qjz.tarul.cn

scp file user@host:/path/
来源：http://znh.shzxlz.cn

[R57] 远程执行命令
来源：http://hja.9152youxi.cn

ssh user@host 'uptime'
来源：http://jep.cdnleiting.top

[R58] 下载文件
来源：http://fmj.jinyuanbaomall.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ivd.zdqjudy.top

[R59] 发 POST JSON
来源：http://mpy.xingfuxueyuan.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lso.ywan-chungtsiang.top

[R60] 只看 HTTP 状态码
来源：http://nux.yuanzhike.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cyu.haohaochexian.top

[R61] 磁盘占用
来源：http://ipd.cucudq.cn


<!-- 参考信息 -->