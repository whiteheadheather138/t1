代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iin.52xcode.cn

[Q18] 模糊匹配
来源：http://wee.snrcjt.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gvr.epnwcf.com

[Q19] 范围查询
来源：http://gtf.guannengcc.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bae.epnwcf.com

[Q20] IN 列表
来源：http://grc.zdbjq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tdq.aibaodan.cn

[Q21] 空值判断
来源：http://pnd.zhaomingkeji.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://gne.bbcook.cn

[Q22] 排序
来源：http://lgo.yanxiufei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ehr.gaohongyu789.top

[Q23] 分页
来源：http://eah.zhoulong.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jrv.chenlongwang.top

[Q24] 去重
来源：http://iew.daxiang520.top

SELECT DISTINCT city FROM users;
来源：http://mcn.cucudq.cn

[Q25] 只取前 N 条
来源：http://bpj.chenzaomai.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hbb.yanxiufei.cn

[Q26] 计数
来源：http://ocp.xylfe.cn

SELECT COUNT(*) FROM users;
来源：http://puh.xziqi.cn

[Q27] 条件计数
来源：http://lms.gogol.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wwp.mhx1999.top

[Q28] 求和与平均
来源：http://rrd.redwolf501.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bcz.sxryk.cn

[Q29] 最大最小值
来源：http://iyl.cdnleiting.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yub.yueranfly.top

[Q30] 分组统计
来源：http://glj.cheryme.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ipx.xuanzx.com

[Q31] 分组后过滤
来源：http://oiw.tanke756.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eqm.sysykeji.top

[Q32] 分组拼接字符串
来源：http://scm.ehwqpu.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uyf.quarkkingdee.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lmo.gzhubu.top

[Q33] 多列分组
来源：http://dre.zhaomingkeji.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kij.zhixingplan.top

[Q34] 每组取第一条
来源：http://kff.hesvh.cn

SELECT * FROM (
来源：http://tms.tarul.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jhi.feifeiyinyue.top

) t WHERE rn = 1;
来源：http://kwk.xingfuxueyuan.xyz

[Q35] 内连接
来源：http://qvc.gaohongyu789.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pdr.yangfankeji.com

[Q36] 左连接
来源：http://wam.bbcook.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://los.hongshengwenyu.top

[Q37] 右连接
来源：http://pwc.316326.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gzu.zdqjudy.top

[Q38] 全外连接（PostgreSQL）
来源：http://pbc.hesvh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lud.yanxiufei.cn

[Q39] 自连接（查上下级）
来源：http://hzb.havefunace.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://uuh.guowangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xvk.52xcode.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://txb.shanyushiyangtech.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://swf.xylfe.cn

[Q41] 多表连接
来源：http://phh.ydzc1.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jmu.sufxvd.cn

JOIN users u ON u.id = o.user_id
来源：http://loo.jiagoushi.top

JOIN products p ON p.id = o.product_id;
来源：http://lvq.cashguo.top

[Q42] 连接条件附加过滤
来源：http://ocq.feifeiyinyue.top

SELECT u.name, o.amount FROM users u
来源：http://mdp.smart0.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ixv.zhongyouzk.top

[Q43] 标量子查询
来源：http://pfv.hongshengwenyu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rnc.zhongyouzk.top

[Q44] IN 子查询
来源：http://bwu.yueranfly.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gsl.nanxuanxn.top

[Q45] EXISTS 判断存在
来源：http://dyg.shanyushiyangtech.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://grd.0kj1m.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vqq.vqdsnc.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fqu.shangyingyoupin.top

[Q47] 与平均值比较
来源：http://ugx.xinyue.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mid.guannengcc.top

[Q48] CTE 公用表表达式
来源：http://eur.havefunace.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nyz.jiagoushi.top

SELECT * FROM t WHERE c > 5;
来源：http://zbv.kuanghao11.cn

[Q49] 更新单行
来源：http://muz.fehbvm.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fto.zhengqikj.top

[Q50] 批量更新
来源：http://imf.zycfv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://egi.sjlbkw.cn

[Q51] 用子查询更新
来源：http://arw.daxiang520.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bnd.haohaochexian.top

[Q52] 删除指定行
来源：http://wvz.feifeiyinyue.top

DELETE FROM users WHERE id = 10;
来源：http://gwu.zycfv.cn

[Q53] 按条件删除
来源：http://qxd.yj202588.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mzn.c1oappe.top

[Q54] 清空表
来源：http://jgr.zhijiandao.cn

TRUNCATE TABLE logs;
来源：http://cxk.pycfn.com

[Q55] 排名（并列占位）
来源：http://jrp.ppjwa.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cbg.wangdashe.top

[Q56] 密集排名（并列不占位）
来源：http://qwj.vqdsnc.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ltb.tarul.cn

[Q57] 行号
来源：http://yhi.yfazqb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eeg.yangfankeji.com

[Q58] 累计求和
来源：http://oxv.zycfv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qml.dashuyun.cn

[Q59] 分组内累计
来源：http://xhw.hywenlv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://aew.316326.xyz

[Q60] 取上一行 / 下一行
来源：http://sdf.ydjk.org.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tqs.yfazqb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mfe.hcnkem.com

[Q61] 移动平均
来源：http://cgh.mhx1999.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://typ.sysykeji.top

[Q62] 分组占比
来源：http://pto.fehbvm.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bxq.jiagoushi.top

[Q63] 开启事务
来源：http://bfg.shanyushiyangtech.top

START TRANSACTION;                -- 或 BEGIN
来源：http://mwa.yj20258.top

[Q64] 提交事务
来源：http://dgj.jianghu66.top

COMMIT;
来源：http://vyk.snrcjt.cn

[Q65] 回滚事务
来源：http://ygf.ywan-chungtsiang.top

ROLLBACK;
来源：http://utz.vqdsnc.cn

[Q66] 行锁查询
来源：http://qkg.jlsjyb.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sqh.hongshengwenyu.top

[Q67] 设置隔离级别
来源：http://sry.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tns.dianchejie.cn

[Q68] 保存点
来源：http://flo.epnwcf.com

SAVEPOINT sp1;
来源：http://jsw.zhixingplan.top

ROLLBACK TO sp1;
来源：http://duh.wangshuangyany.cn

[Q69] 查看执行计划
来源：http://jfj.yuxming.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eer.zhijiandao.cn

[Q70] 更新统计信息
来源：http://cya.hongshengwenyu.top

ANALYZE TABLE users;
来源：http://sih.yanxiufei.cn

[Q71] 查看建表语句
来源：http://niv.bbcook.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://edb.yongpay.top

[Q72] 查看索引
来源：http://rag.xuetiantiany.cn

SHOW INDEX FROM users;
来源：http://izk.yongpay.top

[Q73] 查看表状态
来源：http://dnv.ctjpmb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://dst.zhengqikj.top

[Q74] 强制使用索引
来源：http://nup.sjlbkw.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ivv.jiagoushi.top

[Q75] 日期格式化
来源：http://rer.shanyushiyangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://llp.ppjwa.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wrx.zhongyouzk.top

[Q76] 按天统计
来源：http://kzj.hammf.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nyn.daria6918.cn

[Q77] 时间加减
来源：http://ici.fktsv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://aea.jiagoushi.top

[Q78] 当前时间
来源：http://yze.cdnleiting.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wnn.zdqjudy.top

[Q79] 字符串拼接
来源：http://lwq.316326.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://psd.nwbrower.top

[Q80] 字符串截取
来源：http://qcd.daxiang520.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vyd.nwbrower.top

[Q81] 字符串替换
来源：http://oqy.shanyushiyangtech.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://aqj.gzhubu.top

[Q82] 字符长度与字节长度
来源：http://rbq.bjfxy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ilx.jinqigfzy.top

[Q83] 大小写转换
来源：http://ywc.kuanghao11.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jwj.jinghuilouyu.cn

[Q84] 去除首尾空格
来源：http://blj.shanyushiyangtech.top

SELECT TRIM(name) FROM users;
来源：http://dvb.xuanzx.com

[Q85] 数值取整
来源：http://vgc.ppjwa.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mlc.wangdashe.top

[Q86] 读取 JSON 字段
来源：http://aqz.shangyingyoupin.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eju.bjfxy.top

[Q87] JSON 字段做条件
来源：http://ksd.sufxvd.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qfr.quarkkingdee.top

[Q88] 行转列（条件聚合）
来源：http://lyd.fengsongda.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cyt.tarul.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xqa.jinyuanbaomall.cn

[Q89] 判断表是否存在
来源：http://jwn.nanxinkj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qmd.tanke756.top

[Q90] 生成序号列
来源：http://uyo.cashguo.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wms.mhx1999.top

================================================================================
来源：http://eew.yangfankeji.com

R. Bash 专题
来源：http://wbt.quarkkingdee.top

================================================================================
来源：http://wnm.xinyue.icu

[R01] shebang 与严格模式
来源：http://wsv.yueranfly.top

#!/usr/bin/env bash
来源：http://nlg.jinqigfzy.top

set -euo pipefail
来源：http://bpy.yfazqb.com

[R02] 变量赋值与使用
来源：http://wsg.snrcjt.cn

name="Tom"; echo "$name"
来源：http://mjm.chenzaomai.com

[R03] 只读变量
来源：http://usy.guowangkeji.top

readonly PI=3.14
来源：http://ljw.hongshengwenyu.top

[R04] 位置参数
来源：http://wuk.zhiwuduotai.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mea.xylfe.cn

[R05] 参数默认值
来源：http://qsu.mhx1999.top

name="${1:-default}"
来源：http://kmb.yvedp.cn

[R06] 判断命令是否存在
来源：http://yjb.316326.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ntd.vqdsnc.cn

[R07] if 判断文件
来源：http://zso.chenjidiqi.icu

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oud.hongshengwenyu.top

[R08] 数值比较
来源：http://wtp.pengpengdd.cyou

if (( a > b )); then echo "a 更大"; fi
来源：http://uqk.yanxiufei.cn

[R09] 字符串比较
来源：http://qki.jiagoushi.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://row.dashuyun.cn

[R10] 正则匹配
来源：http://osa.jianghu66.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://izb.ybcxt.top

[R11] case 多分支
来源：http://mak.daxiang520.top

case "$1" in
来源：http://mas.fehbvm.com

start) echo "启动" ;;
来源：http://skz.feifeiyinyue.top

stop)  echo "停止" ;;
来源：http://qyk.tian-w.cn

*)     echo "未知命令" ;;
来源：http://wnk.yj20258.top

esac
来源：http://wjd.vqdsnc.cn

[R12] for 遍历文件
来源：http://ise.zhixingplan.top

for f in *.txt; do echo "$f"; done
来源：http://lux.zhixingplan.top

[R13] for 计数循环
来源：http://rmh.zhoulong.xyz

for i in {1..10}; do echo "$i"; done
来源：http://pga.jyoumei.cn

[R14] C 风格 for
来源：http://rev.zdqjudy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ipd.cashguo.top

[R15] while 逐行读文件
来源：http://fpb.tianlin.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kkj.yj20258888.top

[R16] until 等待条件
来源：http://ldy.c1oappe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wyu.feifeiyinyue.top

[R17] 数组定义与取值
来源：http://ckm.xuetiantiany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pqy.daxiang520.top

[R18] 遍历数组
来源：http://ozx.ywan-chungtsiang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ppq.feifeiyinyue.top

[R19] 数组长度
来源：http://lie.shuidangran.top

echo "${#arr[@]}"
来源：http://ktj.yanxiufei.cn

[R20] 关联数组（字典）
来源：http://zrq.nanxuanxn.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nsq.yuanzhike.top

[R21] 字符串长度
来源：http://oln.yj20258888.top

echo "${#s}"
来源：http://exp.guannengcc.top

[R22] 截取子串
来源：http://cno.cucudq.cn

echo "${s:0:5}"
来源：http://kwe.iojbl.cn

[R23] 字符串替换
来源：http://cck.xziqi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xgq.xziqi.cn

[R24] 大小写转换
来源：http://lnu.yj202588.top

echo "${s^^}"; echo "${s,,}"
来源：http://fwz.yuanzhike.top

[R25] 去后缀 / 去前缀
来源：http://mpf.smart0.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://hqo.yj20258.top

[R26] 命令替换
来源：http://kbq.52xcode.cn

now=$(date +%F); echo "$now"
来源：http://qtb.snrcjt.cn

[R27] 算术展开
来源：http://hqc.tianlin.xyz

echo $((1 + 2 * 3))
来源：http://zpp.yj20258888.top

[R28] 浮点运算
来源：http://yws.jqgfzy.top

echo "scale=2; 10/3" | bc
来源：http://ulb.guowangkeji.top

[R29] 定义函数
来源：http://msx.birdmap.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tyd.dianchejie.cn

[R30] 函数返回状态码
来源：http://kcu.fehbvm.com

f() { return 0; }; f || echo "失败了"
来源：http://zag.sysykeji.top

[R31] 局部变量
来源：http://cvg.guannengcc.top

f() { local x=1; echo "$x"; }
来源：http://jzr.yj202588.top

[R32] 参数个数校验
来源：http://lna.yuxming.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vyx.aibaodan.cn

[R33] 捕获错误并提示行号
来源：http://wnf.zhongyouzk.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://htp.yj20258.top

[R34] 退出时清理
来源：http://lnn.yj20258888.top

trap 'rm -f "$tmp"' EXIT
来源：http://hdc.bbcook.cn

[R35] 后台执行并等待
来源：http://lnj.tianlin.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://uen.ehwqpu.com

[R36] 并发执行多个任务
来源：http://jog.jinqigfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vyn.yuxming.cn

[R37] 把输出赋给变量
来源：http://ojl.uphjek.com

files=$(ls -1)
来源：http://dqm.ydzc1.top

[R38] 管道串联
来源：http://end.c1oappe.top

cat a.txt | grep -i error | wc -l
来源：http://qkw.epnwcf.com

[R39] 重定向标准输出与错误
来源：http://ttq.andypj.xyz

cmd > out.log 2>&1
来源：http://kpr.jinqigfzy.top

[R40] 追加写日志
来源：http://ppc.hongshengwenyu.top

echo "log" >> out.log
来源：http://kbh.pycfn.com

[R41] 丢弃输出
来源：http://gnl.gogol.net.cn

cmd >/dev/null 2>&1
来源：http://enx.ybcxt.top

[R42] 输入重定向
来源：http://ssh.bjfxy.top

wc -l < a.txt
来源：http://jma.hongshengwenyu.top

[R43] 按名字查找文件
来源：http://mrr.fehbvm.com

find . -name "*.log" -type f
来源：http://tbh.0kj1m.cn

[R44] 按修改时间查找
来源：http://yrx.wangdashe.top

find . -mtime -7 -type f
来源：http://aaf.yonumen.top

[R45] 批量删除
来源：http://uip.hcnkem.com

find . -name "*.tmp" -delete
来源：http://rbr.smart0.xyz

[R46] 递归替换文件内容
来源：http://qoh.ydjk.org.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ors.feifeiyinyue.top

[R47] sed 单行替换
来源：http://pyi.chenzaomai.com

sed -i 's/foo/bar/g' a.txt
来源：http://sfw.jianghu66.top

[R48] awk 取指定列
来源：http://uos.snrcjt.cn

awk '{print $1, $3}' a.txt
来源：http://qmw.chenlongwang.top

[R49] awk 带条件
来源：http://fqp.sxryk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qmb.ctjpmb.com

[R50] awk 求和
来源：http://wik.yj20258.top

awk '{s += $2} END {print s}' a.txt
来源：http://map.yuxming.cn

[R51] 排序去重取前几
来源：http://svd.daxiang520.top

sort a.txt | uniq -c | sort -rn | head
来源：http://afw.yangfankeji.com

[R52] 统计行数
来源：http://wms.pengpengdd.cyou

wc -l a.txt
来源：http://shb.yuxming.cn

[R53] 查看文件头与实时尾
来源：http://elg.dashuyun.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aqx.mhx1999.top

[R54] 比较两个文件
来源：http://rju.jinqigfzy.top

diff a.txt b.txt
来源：http://pbx.cashguo.top

[R55] 压缩与解压
来源：http://shd.epnwcf.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fsj.tian-w.cn

[R56] 远程拷贝
来源：http://myy.chenjidiqi.icu

scp file user@host:/path/
来源：http://npj.yvedp.cn

[R57] 远程执行命令
来源：http://ayc.shzxlz.cn

ssh user@host 'uptime'
来源：http://vwe.pengpengdd.cyou

[R58] 下载文件
来源：http://wae.sxryk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yla.0kj1m.cn

[R59] 发 POST JSON
来源：http://swe.9152youxi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baa.yueranfly.top

[R60] 只看 HTTP 状态码
来源：http://dab.havefunace.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qjh.ybcxt.top

[R61] 磁盘占用
来源：http://jfs.yvedp.cn

df -h;  du -sh *
来源：http://zyv.redwolf501.top

[R62] 找最占空间的文件
来源：http://cwy.52xcode.cn

du -ah . | sort -rh | head -10
来源：http://oci.aibaodan.cn

[R63] 内存与进程
来源：http://tlp.epnwcf.com

free -h;  ps aux | grep nginx
来源：http://ypi.uphjek.com

[R64] 结束进程
来源：http://soy.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://sff.jianghu66.top

[R65] 查看端口占用
来源：http://yrt.wangdashe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://niv.0kj1m.cn

[R66] 定时任务
来源：http://ooh.bbcook.cn

crontab -e;  crontab -l
来源：http://ysy.sysykeji.top

[R67] 生成随机十六进制串
来源：http://sma.yuanzhike.top


<!-- 参考信息 -->