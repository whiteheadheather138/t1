代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qpz.xuetiantiany.cn

[Q18] 模糊匹配
来源：http://bmm.pycfn.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kzo.dianchejie.cn

[Q19] 范围查询
来源：http://lyo.zycfv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pyj.kuanghao11.cn

[Q20] IN 列表
来源：http://rbr.redwolf501.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://icd.tarul.cn

[Q21] 空值判断
来源：http://afv.gaohongyu789.top

SELECT * FROM users WHERE email IS NULL;
来源：http://act.sysykeji.top

[Q22] 排序
来源：http://qit.nanxuanxn.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oct.9152youxi.cn

[Q23] 分页
来源：http://cna.shangyingyoupin.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rfu.hysaishi.cn

[Q24] 去重
来源：http://tab.cheryme.top

SELECT DISTINCT city FROM users;
来源：http://jfu.hcnkem.com

[Q25] 只取前 N 条
来源：http://gpw.daxiang520.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dvp.xziqi.cn

[Q26] 计数
来源：http://wvx.daxiang520.top

SELECT COUNT(*) FROM users;
来源：http://uzo.chenzaomai.com

[Q27] 条件计数
来源：http://mjs.fktsv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://stp.gotoacloud.top

[Q28] 求和与平均
来源：http://qnh.xuanzx.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ghg.hammf.cn

[Q29] 最大最小值
来源：http://yhu.xylfe.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qvy.zdbjq.cn

[Q30] 分组统计
来源：http://llu.yvedp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uqw.daria6918.cn

[Q31] 分组后过滤
来源：http://trr.zhiwuduotai.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cpk.shanyushiyangtech.top

[Q32] 分组拼接字符串
来源：http://bbc.yueranfly.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tva.pengpengdd.cyou

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uoh.gotoacloud.top

[Q33] 多列分组
来源：http://akw.cashguo.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fhk.jlsjyb.cn

[Q34] 每组取第一条
来源：http://dye.zhixingplan.top

SELECT * FROM (
来源：http://unz.fanxiaobao.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vfm.birdmap.top

) t WHERE rn = 1;
来源：http://mrd.fanxiaobao.xyz

[Q35] 内连接
来源：http://cas.cashguo.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://grr.ctjpmb.com

[Q36] 左连接
来源：http://uor.sweek.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://csw.nanxinkj.top

[Q37] 右连接
来源：http://hjz.cashguo.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rvw.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://oib.xuetiantiany.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ygy.yuanzhike.top

[Q39] 自连接（查上下级）
来源：http://xfo.hywenlv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wtu.jlsjyb.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ohk.yonumen.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bmy.xuanzx.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cle.zycfv.cn

[Q41] 多表连接
来源：http://lzd.cheryme.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://dhu.aizwys.cn

JOIN users u ON u.id = o.user_id
来源：http://zzt.pengpengdd.cyou

JOIN products p ON p.id = o.product_id;
来源：http://myv.uphjek.com

[Q42] 连接条件附加过滤
来源：http://rmn.vqdsnc.cn

SELECT u.name, o.amount FROM users u
来源：http://fte.hammf.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rpr.cqqwz.cn

[Q43] 标量子查询
来源：http://amf.ydzc1.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hsb.yj20258888.top

[Q44] IN 子查询
来源：http://blb.shuidangran.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kci.ppjwa.cn

[Q45] EXISTS 判断存在
来源：http://vyx.bjfxy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qkg.cqqwz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nxv.nwbrower.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hqw.xziqi.cn

[Q47] 与平均值比较
来源：http://pfc.bjfxy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dmu.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://xxb.hongshengwenyu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://olt.hammf.cn

SELECT * FROM t WHERE c > 5;
来源：http://gsl.bbcook.cn

[Q49] 更新单行
来源：http://bmg.chenzaomai.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hgl.xuanzx.com

[Q50] 批量更新
来源：http://gpv.tian-w.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wym.ivvv.top

[Q51] 用子查询更新
来源：http://ueb.sweek.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://npu.tanke756.top

[Q52] 删除指定行
来源：http://lyw.iojbl.cn

DELETE FROM users WHERE id = 10;
来源：http://imd.fehbvm.com

[Q53] 按条件删除
来源：http://uni.yfazqb.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sob.shanyushiyangkeji.top

[Q54] 清空表
来源：http://rfy.jinqigfzy.top

TRUNCATE TABLE logs;
来源：http://fnj.gotoacloud.top

[Q55] 排名（并列占位）
来源：http://hzx.ivvv.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fti.sweek.top

[Q56] 密集排名（并列不占位）
来源：http://tde.snrcjt.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dbs.tianlin.xyz

[Q57] 行号
来源：http://tux.shanyushiyangkeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://whn.dashuyun.cn

[Q58] 累计求和
来源：http://kyr.zdqjudy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kjl.gogol.net.cn

[Q59] 分组内累计
来源：http://ekf.sufxvd.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jdu.shzxlz.cn

[Q60] 取上一行 / 下一行
来源：http://ams.hysaishi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rmz.birdmap.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://and.yfazqb.com

[Q61] 移动平均
来源：http://ytw.ywan-chungtsiang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mra.redwolf501.top

[Q62] 分组占比
来源：http://jxk.hcnkem.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vjr.smart0.xyz

[Q63] 开启事务
来源：http://isk.gaohongyu789.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wyy.xziqi.cn

[Q64] 提交事务
来源：http://ncd.hesvh.cn

COMMIT;
来源：http://wun.jinqigufen.top

[Q65] 回滚事务
来源：http://nrp.feifeiyinyue.top

ROLLBACK;
来源：http://lgd.jinqigfzy.top

[Q66] 行锁查询
来源：http://jmn.ybcxt.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ydb.jqgufenzy.top

[Q67] 设置隔离级别
来源：http://fmj.sufxvd.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fyd.chenzaomai.com

[Q68] 保存点
来源：http://zwi.bjfxy.top

SAVEPOINT sp1;
来源：http://riu.jlsjyb.cn

ROLLBACK TO sp1;
来源：http://mkk.bbcook.cn

[Q69] 查看执行计划
来源：http://err.sysykeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://irb.yuanzhike.top

[Q70] 更新统计信息
来源：http://ttr.yonumen.top

ANALYZE TABLE users;
来源：http://hkl.sweek.top

[Q71] 查看建表语句
来源：http://bhq.yj202588.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uhk.wangshuangyany.cn

[Q72] 查看索引
来源：http://nkb.wangdashe.top

SHOW INDEX FROM users;
来源：http://tyw.quarkkingdee.top

[Q73] 查看表状态
来源：http://phf.jinqigfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wmo.bbcook.cn

[Q74] 强制使用索引
来源：http://nsk.jiagoushi.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ser.c1oappe.top

[Q75] 日期格式化
来源：http://gry.ivvv.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ebt.9152youxi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://stv.fehbvm.com

[Q76] 按天统计
来源：http://lcu.bbcook.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dks.jinghuilouyu.cn

[Q77] 时间加减
来源：http://ebs.hnxiangtu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://odi.wangdashe.top

[Q78] 当前时间
来源：http://hss.xylfe.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pxo.ppjwa.cn

[Q79] 字符串拼接
来源：http://sjk.dashuyun.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bvt.shangyingyoupin.top

[Q80] 字符串截取
来源：http://tfn.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ziu.ivvv.top

[Q81] 字符串替换
来源：http://dhx.fengsongda.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://obh.316326.xyz

[Q82] 字符长度与字节长度
来源：http://nff.zhixingplan.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ajs.xingfuxueyuan.xyz

[Q83] 大小写转换
来源：http://oxz.fehbvm.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mbd.cqqwz.cn

[Q84] 去除首尾空格
来源：http://erl.nanxinkj.top

SELECT TRIM(name) FROM users;
来源：http://urh.nanxuanxn.top

[Q85] 数值取整
来源：http://vlu.yj20258888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ede.ppjwa.cn

[Q86] 读取 JSON 字段
来源：http://tli.daria6918.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wxe.redwolf501.top

[Q87] JSON 字段做条件
来源：http://kqt.ppjwa.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qcf.yonumen.top

[Q88] 行转列（条件聚合）
来源：http://dzd.chenzaomai.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cbe.iojbl.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zyt.zhiwuduotai.top

[Q89] 判断表是否存在
来源：http://dzq.9152youxi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wzf.ydzc1.top

[Q90] 生成序号列
来源：http://anx.sjlbkw.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uqj.aibaodan.cn

================================================================================
来源：http://xvx.sjlbkw.cn

R. Bash 专题
来源：http://yft.ydjk.org.cn

================================================================================
来源：http://qfq.daria6918.cn

[R01] shebang 与严格模式
来源：http://ngg.jiagoushi.top

#!/usr/bin/env bash
来源：http://bmo.yongpay.top

set -euo pipefail
来源：http://jud.smart0.xyz

[R02] 变量赋值与使用
来源：http://xrx.jlsjyb.cn

name="Tom"; echo "$name"
来源：http://iak.hammf.cn

[R03] 只读变量
来源：http://rix.jinqigufen.top

readonly PI=3.14
来源：http://qat.ydzc1.top

[R04] 位置参数
来源：http://zwp.xinyue.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://frx.shzxlz.cn

[R05] 参数默认值
来源：http://cyc.jinghuilouyu.cn

name="${1:-default}"
来源：http://aqp.snrcjt.cn

[R06] 判断命令是否存在
来源：http://hbp.nanxuanxn.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zlw.cdnleiting.top

[R07] if 判断文件
来源：http://gqc.xziqi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://afs.ywan-chungtsiang.top

[R08] 数值比较
来源：http://fgk.epnwcf.com

if (( a > b )); then echo "a 更大"; fi
来源：http://dvy.mhx1999.top

[R09] 字符串比较
来源：http://wer.meibo888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dzy.fktsv.cn

[R10] 正则匹配
来源：http://pke.zhiwuduotai.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://avc.smart0.xyz

[R11] case 多分支
来源：http://vpu.hysaishi.cn

case "$1" in
来源：http://npm.xylfe.cn

start) echo "启动" ;;
来源：http://hlm.birdmap.top

stop)  echo "停止" ;;
来源：http://nix.hammf.cn

*)     echo "未知命令" ;;
来源：http://paf.cucudq.cn

esac
来源：http://gua.daria6918.cn

[R12] for 遍历文件
来源：http://rom.smart0.xyz

for f in *.txt; do echo "$f"; done
来源：http://uyu.jianghu66.top

[R13] for 计数循环
来源：http://pmv.shangyingyoupin.top

for i in {1..10}; do echo "$i"; done
来源：http://uho.mhx1999.top

[R14] C 风格 for
来源：http://gcl.feifeiyinyue.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sbn.gzhubu.top

[R15] while 逐行读文件
来源：http://sqm.316326.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ytp.sxryk.cn

[R16] until 等待条件
来源：http://dar.zhiwuduotai.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://swf.gzhubu.top

[R17] 数组定义与取值
来源：http://vyz.jinqigufen.top

arr=(a b c); echo "${arr[0]}"
来源：http://dno.wangshuangyany.cn

[R18] 遍历数组
来源：http://mca.yj20258888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://msy.aizwys.cn

[R19] 数组长度
来源：http://enu.zhengqikj.top

echo "${#arr[@]}"
来源：http://aja.fktsv.cn

[R20] 关联数组（字典）
来源：http://elq.svipenyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zuq.sysykeji.top

[R21] 字符串长度
来源：http://fyl.shanyushiyangkeji.top

echo "${#s}"
来源：http://zlq.aibaodan.cn

[R22] 截取子串
来源：http://rau.zycfv.cn

echo "${s:0:5}"
来源：http://rip.aibaodan.cn

[R23] 字符串替换
来源：http://urm.gaohongyu789.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zej.xuetiantiany.cn

[R24] 大小写转换
来源：http://jxb.nanxinkj.top

echo "${s^^}"; echo "${s,,}"
来源：http://ylq.jinyuanbaomall.cn

[R25] 去后缀 / 去前缀
来源：http://qar.ivvv.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lpj.ywan-chungtsiang.top

[R26] 命令替换
来源：http://soy.ivvv.top

now=$(date +%F); echo "$now"
来源：http://yyd.epnwcf.com

[R27] 算术展开
来源：http://dus.ydzc1.top

echo $((1 + 2 * 3))
来源：http://ygl.sxryk.cn

[R28] 浮点运算
来源：http://hlm.xziqi.cn

echo "scale=2; 10/3" | bc
来源：http://ibo.hongshengwenyu.top

[R29] 定义函数
来源：http://zjo.fehbvm.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yzh.zycfv.cn

[R30] 函数返回状态码
来源：http://zlm.bjfxy.top

f() { return 0; }; f || echo "失败了"
来源：http://krd.tanke756.top

[R31] 局部变量
来源：http://prp.zhixingplan.top

f() { local x=1; echo "$x"; }
来源：http://xmj.havefunace.top

[R32] 参数个数校验
来源：http://cen.dashuyun.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uhz.zdbjq.cn

[R33] 捕获错误并提示行号
来源：http://jnj.xuanzx.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wkj.xziqi.cn

[R34] 退出时清理
来源：http://yqm.shangyingyoupin.top

trap 'rm -f "$tmp"' EXIT
来源：http://rau.redwolf501.top

[R35] 后台执行并等待
来源：http://pua.yuanzhike.top

sleep 5 & pid=$!; wait "$pid"
来源：http://cmc.gotoacloud.top

[R36] 并发执行多个任务
来源：http://syk.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://soq.zhixingplan.top

[R37] 把输出赋给变量
来源：http://agl.hnxiangtu.top

files=$(ls -1)
来源：http://stb.vehdjk.com

[R38] 管道串联
来源：http://vel.chenjidiqi.icu

cat a.txt | grep -i error | wc -l
来源：http://kwk.birdmap.top

[R39] 重定向标准输出与错误
来源：http://xzu.ivvv.top

cmd > out.log 2>&1
来源：http://ylr.wangshuangyany.cn

[R40] 追加写日志
来源：http://srs.ehwqpu.com

echo "log" >> out.log
来源：http://prj.ehwqpu.com

[R41] 丢弃输出
来源：http://yyx.zhijiandao.cn

cmd >/dev/null 2>&1
来源：http://fbx.fanxiaobao.xyz

[R42] 输入重定向
来源：http://xoi.haohaochexian.top

wc -l < a.txt
来源：http://lzx.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://xxq.xuetiantiany.cn

find . -name "*.log" -type f
来源：http://isf.jlsjyb.cn

[R44] 按修改时间查找
来源：http://ort.yongpay.top

find . -mtime -7 -type f
来源：http://dcw.xziqi.cn

[R45] 批量删除
来源：http://amd.ehwqpu.com

find . -name "*.tmp" -delete
来源：http://fww.0kj1m.cn

[R46] 递归替换文件内容
来源：http://lni.jinqigfzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jam.jianghu66.top

[R47] sed 单行替换
来源：http://ncd.xingfuxueyuan.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://kte.jianghu66.top

[R48] awk 取指定列
来源：http://ond.dianchejie.cn

awk '{print $1, $3}' a.txt
来源：http://rif.zhixingplan.top

[R49] awk 带条件
来源：http://vbt.zhoulong.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://puv.cdnleiting.top

[R50] awk 求和
来源：http://qco.chenlongwang.top

awk '{s += $2} END {print s}' a.txt
来源：http://joj.yvedp.cn

[R51] 排序去重取前几
来源：http://lhd.redwolf501.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bjv.vehdjk.com

[R52] 统计行数
来源：http://wta.hywenlv.cn

wc -l a.txt
来源：http://ipf.andypj.xyz

[R53] 查看文件头与实时尾
来源：http://zcl.svipenyu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jzz.sufxvd.cn

[R54] 比较两个文件
来源：http://ptj.dianchejie.cn

diff a.txt b.txt
来源：http://fsd.zhijiandao.cn

[R55] 压缩与解压
来源：http://ixx.yuanzhike.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qge.jinghuilouyu.cn

[R56] 远程拷贝
来源：http://wzg.fktsv.cn

scp file user@host:/path/
来源：http://rpy.cucudq.cn

[R57] 远程执行命令
来源：http://ivb.ybcxt.top

ssh user@host 'uptime'
来源：http://qxe.vehdjk.com

[R58] 下载文件
来源：http://xwn.birdmap.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ygh.sjlbkw.cn

[R59] 发 POST JSON
来源：http://aem.xuetiantiany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dyg.vehdjk.com

[R60] 只看 HTTP 状态码
来源：http://xmt.bjfxy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vud.vehdjk.com

[R61] 磁盘占用
来源：http://nzz.tianlin.xyz

df -h;  du -sh *
来源：http://woz.redwolf501.top

[R62] 找最占空间的文件
来源：http://enm.jinyuanbaomall.cn

du -ah . | sort -rh | head -10
来源：http://lcm.daxiang520.top

[R63] 内存与进程
来源：http://mzg.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://dys.hfpthk.cn

[R64] 结束进程
来源：http://stj.0kj1m.cn

kill -9 $(pgrep -f app.py)
来源：http://ujc.yueranfly.top

[R65] 查看端口占用
来源：http://jow.gaohongyu789.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dsj.xinyue.icu

[R66] 定时任务
来源：http://ien.yueranfly.top

crontab -e;  crontab -l
来源：http://icc.yj202588.top

[R67] 生成随机十六进制串
来源：http://ykn.zhiwuduotai.top


<!-- 参考信息 -->