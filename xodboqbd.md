代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://poi.tianlin.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://udc.gzhubu.top

[Q13] 忽略重复插入
来源：http://tda.shanyushiyangtech.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uyc.meibo888.top

[Q14] 存在则更新（upsert）
来源：http://vug.gzhubu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qks.hysaishi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mrq.tianlin.xyz

[Q15] 查询全部
来源：http://hql.gaohongyu789.top

SELECT * FROM users;
来源：http://flx.yongpay.top

[Q16] 查询指定列
来源：http://nvt.xuanzx.com

SELECT id, name FROM users;
来源：http://gge.yj20258.top

[Q17] 条件查询
来源：http://fpo.nanxuanxn.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wmm.sxryk.cn

[Q18] 模糊匹配
来源：http://eoa.dianchejie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ynr.hysaishi.cn

[Q19] 范围查询
来源：http://iqd.hywenlv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lpk.pycfn.com

[Q20] IN 列表
来源：http://mok.dashuyun.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ali.xuanzx.com

[Q21] 空值判断
来源：http://hvc.tanke756.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bzj.fzhhl.top

[Q22] 排序
来源：http://gqm.hcnkem.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mix.bbcook.cn

[Q23] 分页
来源：http://jpc.daria6918.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://spt.cucudq.cn

[Q24] 去重
来源：http://fdw.uphjek.com

SELECT DISTINCT city FROM users;
来源：http://dbn.sweek.top

[Q25] 只取前 N 条
来源：http://zyl.hywenlv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hck.xuetiantiany.cn

[Q26] 计数
来源：http://gfz.vehdjk.com

SELECT COUNT(*) FROM users;
来源：http://jrr.gzhubu.top

[Q27] 条件计数
来源：http://nqh.zhixingplan.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pzr.nanxuanxn.top

[Q28] 求和与平均
来源：http://wot.jinyuanbaomall.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://smp.ybcxt.top

[Q29] 最大最小值
来源：http://vbj.sweek.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://rec.gaohongyu789.top

[Q30] 分组统计
来源：http://gvu.yj202588.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hcj.jinqigfzy.top

[Q31] 分组后过滤
来源：http://nmg.kuanghao11.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mfj.yj20258888.top

[Q32] 分组拼接字符串
来源：http://iyu.yfazqb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://scj.guannengcc.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uvt.cqqwz.cn

[Q33] 多列分组
来源：http://uhc.hfpthk.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jcl.daria6918.cn

[Q34] 每组取第一条
来源：http://hls.ydzc1.top

SELECT * FROM (
来源：http://bkm.yueranfly.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://biy.nwbrower.top

) t WHERE rn = 1;
来源：http://mzk.uphjek.com

[Q35] 内连接
来源：http://ebx.hnxiangtu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ego.fanxiaobao.xyz

[Q36] 左连接
来源：http://gwh.sweek.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rhw.zhengqikj.top

[Q37] 右连接
来源：http://zvk.shuidangran.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rjw.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wxs.quarkkingdee.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://exk.cashguo.top

[Q39] 自连接（查上下级）
来源：http://ble.jiagoushi.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qxt.cdnleiting.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kji.yanxiufei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xex.ctjpmb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nvz.xuetiantiany.cn

[Q41] 多表连接
来源：http://wdc.svipenyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bzj.epnwcf.com

JOIN users u ON u.id = o.user_id
来源：http://pzy.zhongyouzk.top

JOIN products p ON p.id = o.product_id;
来源：http://ltt.jinyuanbaomall.cn

[Q42] 连接条件附加过滤
来源：http://szv.gotoacloud.top

SELECT u.name, o.amount FROM users u
来源：http://hrv.gogol.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xmc.0kj1m.cn

[Q43] 标量子查询
来源：http://dmn.hnqzz.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fzo.ppjwa.cn

[Q44] IN 子查询
来源：http://jaj.cdnleiting.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rti.yanxiufei.cn

[Q45] EXISTS 判断存在
来源：http://bkx.zhijiandao.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://awu.yonumen.top

[Q46] NOT EXISTS 判断不存在
来源：http://oea.ybcxt.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nge.meibo888.top

[Q47] 与平均值比较
来源：http://lat.yvedp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mee.cucudq.cn

[Q48] CTE 公用表表达式
来源：http://zof.gaohongyu789.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tnd.gaohongyu789.top

SELECT * FROM t WHERE c > 5;
来源：http://xid.quarkkingdee.top

[Q49] 更新单行
来源：http://cwj.meibo888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://edd.shanyushiyangtech.top

[Q50] 批量更新
来源：http://pne.zdbjq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mxr.hnxiangtu.top

[Q51] 用子查询更新
来源：http://fal.shanyushiyangtech.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vag.gotoacloud.top

[Q52] 删除指定行
来源：http://awd.zycfv.cn

DELETE FROM users WHERE id = 10;
来源：http://olg.ivvv.top

[Q53] 按条件删除
来源：http://yfp.zhongyouzk.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qem.ydjk.org.cn

[Q54] 清空表
来源：http://yue.zycfv.cn

TRUNCATE TABLE logs;
来源：http://feb.zhengqikj.top

[Q55] 排名（并列占位）
来源：http://jve.ehwqpu.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wxd.vehdjk.com

[Q56] 密集排名（并列不占位）
来源：http://hsp.cdnleiting.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dwp.hammf.cn

[Q57] 行号
来源：http://ekf.hnxiangtu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eko.yfazqb.com

[Q58] 累计求和
来源：http://jod.yueranfly.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wxl.zhiwuduotai.top

[Q59] 分组内累计
来源：http://ioz.yangfankeji.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://aih.aizwys.cn

[Q60] 取上一行 / 下一行
来源：http://pqh.yj20258888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gry.ywan-chungtsiang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bmk.yj202588.top

[Q61] 移动平均
来源：http://ybv.xuanzx.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xxs.yangfankeji.com

[Q62] 分组占比
来源：http://jyg.shzxlz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tnq.andypj.xyz

[Q63] 开启事务
来源：http://rxv.xinyue.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://rhc.hammf.cn

[Q64] 提交事务
来源：http://izy.fengsongda.top

COMMIT;
来源：http://ubh.tanke756.top

[Q65] 回滚事务
来源：http://inl.chenzaomai.com

ROLLBACK;
来源：http://ykx.52xcode.cn

[Q66] 行锁查询
来源：http://xmg.cqqwz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wlq.xylfe.cn

[Q67] 设置隔离级别
来源：http://maf.cashguo.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dri.hammf.cn

[Q68] 保存点
来源：http://kaw.dashuyun.cn

SAVEPOINT sp1;
来源：http://cne.jyoumei.cn

ROLLBACK TO sp1;
来源：http://tpx.pycfn.com

[Q69] 查看执行计划
来源：http://zsd.kuanghao11.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://owk.shangyingyoupin.top

[Q70] 更新统计信息
来源：http://jfd.shzxlz.cn

ANALYZE TABLE users;
来源：http://zto.shanyushiyangtech.top

[Q71] 查看建表语句
来源：http://hty.fzhhl.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nqp.jianghu66.top

[Q72] 查看索引
来源：http://ohy.zycfv.cn

SHOW INDEX FROM users;
来源：http://cps.jqgfzy.top

[Q73] 查看表状态
来源：http://uds.ybcxt.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mcy.yuanzhike.top

[Q74] 强制使用索引
来源：http://ugj.jiagoushi.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qgg.snrcjt.cn

[Q75] 日期格式化
来源：http://xyl.iojbl.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ail.aibaodan.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://txb.nanxuanxn.top

[Q76] 按天统计
来源：http://cax.cheryme.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ecr.shuidangran.top

[Q77] 时间加减
来源：http://vqn.svipenyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wab.cucudq.cn

[Q78] 当前时间
来源：http://hhe.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://psq.vehdjk.com

[Q79] 字符串拼接
来源：http://kyk.hysaishi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kzg.fehbvm.com

[Q80] 字符串截取
来源：http://ich.zhixingplan.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xin.xziqi.cn

[Q81] 字符串替换
来源：http://vel.jinyuanbaomall.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ika.bbcook.cn

[Q82] 字符长度与字节长度
来源：http://xxz.yuxming.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qij.xinyue.icu

[Q83] 大小写转换
来源：http://hdp.yj20258.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gwv.guannengcc.top

[Q84] 去除首尾空格
来源：http://laz.zhengqikj.top

SELECT TRIM(name) FROM users;
来源：http://zbh.yj20258.top

[Q85] 数值取整
来源：http://cdj.quarkkingdee.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hxp.zhijiandao.cn

[Q86] 读取 JSON 字段
来源：http://wgi.dashuyun.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rju.yonumen.top

[Q87] JSON 字段做条件
来源：http://ssv.fzhhl.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dms.fengsongda.top

[Q88] 行转列（条件聚合）
来源：http://jjb.ybcxt.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rfc.yj202588.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zmb.gogol.net.cn

[Q89] 判断表是否存在
来源：http://rvt.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vwr.hnqzz.top

[Q90] 生成序号列
来源：http://lll.ivvv.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qho.cqqwz.cn

================================================================================
来源：http://ino.fzhhl.top

R. Bash 专题
来源：http://kfi.epnwcf.com

================================================================================
来源：http://haf.yonumen.top

[R01] shebang 与严格模式
来源：http://tbu.jianghu66.top

#!/usr/bin/env bash
来源：http://snf.hfpthk.cn

set -euo pipefail
来源：http://bvg.sjlbkw.cn

[R02] 变量赋值与使用
来源：http://thb.zhengqikj.top

name="Tom"; echo "$name"
来源：http://siv.ywan-chungtsiang.top

[R03] 只读变量
来源：http://umv.zycfv.cn

readonly PI=3.14
来源：http://uyc.yangfankeji.com

[R04] 位置参数
来源：http://dlg.nanxuanxn.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://djp.vqdsnc.cn

[R05] 参数默认值
来源：http://yfm.yj202588.top

name="${1:-default}"
来源：http://wmq.0kj1m.cn

[R06] 判断命令是否存在
来源：http://nqn.chenjidiqi.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://udl.cqqwz.cn

[R07] if 判断文件
来源：http://emp.zhixingplan.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hia.andypj.xyz

[R08] 数值比较
来源：http://dnq.yonumen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vps.gogol.net.cn

[R09] 字符串比较
来源：http://jua.dashuyun.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bzp.zycfv.cn

[R10] 正则匹配
来源：http://vjs.hnxiangtu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wns.ppjwa.cn

[R11] case 多分支
来源：http://zjw.52xcode.cn

case "$1" in
来源：http://wlf.jinqigufen.top

start) echo "启动" ;;
来源：http://lrp.sxryk.cn

stop)  echo "停止" ;;
来源：http://wru.daxiang520.top

*)     echo "未知命令" ;;
来源：http://ygr.vehdjk.com

esac
来源：http://vsk.hywenlv.cn

[R12] for 遍历文件
来源：http://apj.snrcjt.cn

for f in *.txt; do echo "$f"; done
来源：http://ths.yueranfly.top

[R13] for 计数循环
来源：http://cpi.zhongyouzk.top

for i in {1..10}; do echo "$i"; done
来源：http://ohc.chenlongwang.top

[R14] C 风格 for
来源：http://csd.jinqigufen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gks.zhengqikj.top

[R15] while 逐行读文件
来源：http://lcp.jiagoushi.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ivx.zhijiandao.cn

[R16] until 等待条件
来源：http://iqc.zdbjq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zbp.gzhubu.top

[R17] 数组定义与取值
来源：http://rpf.xylfe.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rfi.nanxuanxn.top

[R18] 遍历数组
来源：http://une.zhoulong.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rtv.andypj.xyz

[R19] 数组长度
来源：http://jnr.sjlbkw.cn

echo "${#arr[@]}"
来源：http://jdj.ywan-chungtsiang.top

[R20] 关联数组（字典）
来源：http://zmm.aizwys.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://htj.ybcxt.top

[R21] 字符串长度
来源：http://hhd.birdmap.top

echo "${#s}"
来源：http://thl.yvedp.cn

[R22] 截取子串
来源：http://vit.yanxiufei.cn

echo "${s:0:5}"
来源：http://bec.xingfuxueyuan.xyz

[R23] 字符串替换
来源：http://tan.sufxvd.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vcj.fengsongda.top

[R24] 大小写转换
来源：http://krs.meibo888.top

echo "${s^^}"; echo "${s,,}"
来源：http://joy.gaohongyu789.top

[R25] 去后缀 / 去前缀
来源：http://bae.yfazqb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://ngd.c1oappe.top

[R26] 命令替换
来源：http://qxx.hywenlv.cn

now=$(date +%F); echo "$now"
来源：http://kgx.mhx1999.top

[R27] 算术展开
来源：http://xaz.shuidangran.top

echo $((1 + 2 * 3))
来源：http://jah.cashguo.top

[R28] 浮点运算
来源：http://pgd.guowangkeji.top

echo "scale=2; 10/3" | bc
来源：http://djf.cdnleiting.top

[R29] 定义函数
来源：http://jbw.guannengcc.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pfb.ivvv.top

[R30] 函数返回状态码
来源：http://fpc.svipenyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://bpi.sysykeji.top

[R31] 局部变量
来源：http://asj.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://hxz.guowangkeji.top

[R32] 参数个数校验
来源：http://mra.zhiwuduotai.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://prn.ehwqpu.com

[R33] 捕获错误并提示行号
来源：http://qzc.yfazqb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bmg.uphjek.com

[R34] 退出时清理
来源：http://lss.shangyingyoupin.top

trap 'rm -f "$tmp"' EXIT
来源：http://fha.fzhhl.top

[R35] 后台执行并等待
来源：http://dut.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rmx.sweek.top

[R36] 并发执行多个任务
来源：http://qay.tianlin.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xtv.ivvv.top

[R37] 把输出赋给变量
来源：http://ntx.0kj1m.cn

files=$(ls -1)
来源：http://nay.tianlin.xyz

[R38] 管道串联
来源：http://zzl.hysaishi.cn

cat a.txt | grep -i error | wc -l
来源：http://roq.zhijiandao.cn

[R39] 重定向标准输出与错误
来源：http://ohq.quarkkingdee.top

cmd > out.log 2>&1
来源：http://kul.nwbrower.top

[R40] 追加写日志
来源：http://vrr.gotoacloud.top

echo "log" >> out.log
来源：http://ocd.sxryk.cn

[R41] 丢弃输出
来源：http://gea.ctjpmb.com

cmd >/dev/null 2>&1
来源：http://nzz.sysykeji.top

[R42] 输入重定向
来源：http://tik.gzhubu.top

wc -l < a.txt
来源：http://nhr.sysykeji.top

[R43] 按名字查找文件
来源：http://kvy.havefunace.top

find . -name "*.log" -type f
来源：http://qie.hesvh.cn

[R44] 按修改时间查找
来源：http://uvk.aizwys.cn

find . -mtime -7 -type f
来源：http://emo.yuxming.cn

[R45] 批量删除
来源：http://loa.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://aqx.fktsv.cn

[R46] 递归替换文件内容
来源：http://xmv.shzxlz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nue.hammf.cn

[R47] sed 单行替换
来源：http://lzh.bbcook.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jjt.xziqi.cn

[R48] awk 取指定列
来源：http://imt.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://gef.guannengcc.top

[R49] awk 带条件
来源：http://flt.quarkkingdee.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mck.smart0.xyz

[R50] awk 求和
来源：http://fpt.jinyuanbaomall.cn

awk '{s += $2} END {print s}' a.txt
来源：http://awt.aizwys.cn

[R51] 排序去重取前几
来源：http://oav.zycfv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mba.pycfn.com

[R52] 统计行数
来源：http://okf.guannengcc.top

wc -l a.txt
来源：http://rhf.sufxvd.cn

[R53] 查看文件头与实时尾
来源：http://eoi.yanxiufei.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://foz.hesvh.cn

[R54] 比较两个文件
来源：http://lkw.hnxiangtu.top

diff a.txt b.txt
来源：http://ibm.tarul.cn

[R55] 压缩与解压
来源：http://bsv.shzxlz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rwt.nanxuanxn.top

[R56] 远程拷贝
来源：http://zef.yfazqb.com

scp file user@host:/path/
来源：http://ldc.yueranfly.top

[R57] 远程执行命令
来源：http://str.shzxlz.cn

ssh user@host 'uptime'
来源：http://kel.redwolf501.top

[R58] 下载文件
来源：http://hlg.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pjd.yj20258.top

[R59] 发 POST JSON
来源：http://izz.shanyushiyangtech.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vky.jinqigfzy.top

[R60] 只看 HTTP 状态码
来源：http://sfw.sweek.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ajg.jiagoushi.top

[R61] 磁盘占用
来源：http://eug.yuxming.cn


<!-- 参考信息 -->