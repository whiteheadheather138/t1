代发 wailian999

SELECT * FROM users;
来源：http://psr.ydzc1.top

[Q16] 查询指定列
来源：http://oei.yj20258.top

SELECT id, name FROM users;
来源：http://dit.sweek.top

[Q17] 条件查询
来源：http://zus.fktsv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cbl.yueranfly.top

[Q18] 模糊匹配
来源：http://jgx.epnwcf.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xme.ybcxt.top

[Q19] 范围查询
来源：http://xkm.zhixingplan.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lae.ivvv.top

[Q20] IN 列表
来源：http://ikr.jianghu66.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jkl.aizwys.cn

[Q21] 空值判断
来源：http://pac.nwbrower.top

SELECT * FROM users WHERE email IS NULL;
来源：http://exc.c1oappe.top

[Q22] 排序
来源：http://suq.zhaomingkeji.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dsm.birdmap.top

[Q23] 分页
来源：http://mbu.hesvh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dcv.hfpthk.cn

[Q24] 去重
来源：http://qgy.hfpthk.cn

SELECT DISTINCT city FROM users;
来源：http://pop.quarkkingdee.top

[Q25] 只取前 N 条
来源：http://lut.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://olz.yj202588.top

[Q26] 计数
来源：http://ngs.nanxinkj.top

SELECT COUNT(*) FROM users;
来源：http://uvp.yj202588.top

[Q27] 条件计数
来源：http://bci.jinghuilouyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vzz.yueranfly.top

[Q28] 求和与平均
来源：http://dqc.zhoulong.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://shz.chenjidiqi.icu

[Q29] 最大最小值
来源：http://vaf.ppjwa.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qtn.sxryk.cn

[Q30] 分组统计
来源：http://htt.guannengcc.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jar.shanyushiyangkeji.top

[Q31] 分组后过滤
来源：http://opn.redwolf501.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://iva.fzhhl.top

[Q32] 分组拼接字符串
来源：http://fpw.cucudq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mmf.sxryk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vhz.andypj.xyz

[Q33] 多列分组
来源：http://yho.wangdashe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lkw.fanxiaobao.xyz

[Q34] 每组取第一条
来源：http://pde.guowangkeji.top

SELECT * FROM (
来源：http://bhm.gaohongyu789.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://heb.wangdashe.top

) t WHERE rn = 1;
来源：http://qhi.0kj1m.cn

[Q35] 内连接
来源：http://drl.wangdashe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ftl.zdqjudy.top

[Q36] 左连接
来源：http://tgz.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wxq.hnqzz.top

[Q37] 右连接
来源：http://hjh.xinyue.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yvb.ctjpmb.com

[Q38] 全外连接（PostgreSQL）
来源：http://hhm.cucudq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gkh.yueranfly.top

[Q39] 自连接（查上下级）
来源：http://utr.gotoacloud.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xvu.chenlongwang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ofb.ydjk.org.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rqm.zhijiandao.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qbs.jlsjyb.cn

[Q41] 多表连接
来源：http://kgh.9152youxi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ols.zhixingplan.top

JOIN users u ON u.id = o.user_id
来源：http://cnu.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://caw.hammf.cn

[Q42] 连接条件附加过滤
来源：http://exs.sweek.top

SELECT u.name, o.amount FROM users u
来源：http://aqv.chenlongwang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mhw.feifeiyinyue.top

[Q43] 标量子查询
来源：http://tzg.jianghu66.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://otj.meibo888.top

[Q44] IN 子查询
来源：http://wvn.zhiwuduotai.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sbd.jyoumei.cn

[Q45] EXISTS 判断存在
来源：http://iga.yfazqb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cju.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://ioi.0kj1m.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eut.zhengqikj.top

[Q47] 与平均值比较
来源：http://aig.hywenlv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wwy.hcnkem.com

[Q48] CTE 公用表表达式
来源：http://xhf.zdbjq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vea.sysykeji.top

SELECT * FROM t WHERE c > 5;
来源：http://gup.guannengcc.top

[Q49] 更新单行
来源：http://agt.gotoacloud.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xek.yuxming.cn

[Q50] 批量更新
来源：http://mnm.cdnleiting.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zzv.tianlin.xyz

[Q51] 用子查询更新
来源：http://rdd.jlsjyb.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://myi.gzhubu.top

[Q52] 删除指定行
来源：http://brb.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://gyx.chenjidiqi.icu

[Q53] 按条件删除
来源：http://fjf.chenzaomai.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lhj.shanyushiyangtech.top

[Q54] 清空表
来源：http://qfp.xziqi.cn

TRUNCATE TABLE logs;
来源：http://chv.daria6918.cn

[Q55] 排名（并列占位）
来源：http://zik.redwolf501.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nmr.pycfn.com

[Q56] 密集排名（并列不占位）
来源：http://ufk.hysaishi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kyj.chenlongwang.top

[Q57] 行号
来源：http://ubd.jinyuanbaomall.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mpt.bjfxy.top

[Q58] 累计求和
来源：http://pgq.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ppm.nanxinkj.top

[Q59] 分组内累计
来源：http://vkf.chenzaomai.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qqo.xziqi.cn

[Q60] 取上一行 / 下一行
来源：http://lta.zhixingplan.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fvb.jinyuanbaomall.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gsb.zhengqikj.top

[Q61] 移动平均
来源：http://jlp.fzhhl.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vme.hywenlv.cn

[Q62] 分组占比
来源：http://hsj.redwolf501.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sgu.shanyushiyangtech.top

[Q63] 开启事务
来源：http://bzl.chenzaomai.com

START TRANSACTION;                -- 或 BEGIN
来源：http://mxg.52xcode.cn

[Q64] 提交事务
来源：http://mah.yj202588.top

COMMIT;
来源：http://hzp.mhx1999.top

[Q65] 回滚事务
来源：http://nvr.hywenlv.cn

ROLLBACK;
来源：http://ryn.yonumen.top

[Q66] 行锁查询
来源：http://vdo.feifeiyinyue.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zpl.redwolf501.top

[Q67] 设置隔离级别
来源：http://fkm.andypj.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bkm.c1oappe.top

[Q68] 保存点
来源：http://uid.yonumen.top

SAVEPOINT sp1;
来源：http://six.dianchejie.cn

ROLLBACK TO sp1;
来源：http://aoc.aibaodan.cn

[Q69] 查看执行计划
来源：http://pst.xingfuxueyuan.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vxb.cashguo.top

[Q70] 更新统计信息
来源：http://ixz.xinyue.icu

ANALYZE TABLE users;
来源：http://enl.shzxlz.cn

[Q71] 查看建表语句
来源：http://rgf.birdmap.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bwc.gzhubu.top

[Q72] 查看索引
来源：http://wyc.hysaishi.cn

SHOW INDEX FROM users;
来源：http://mpc.xingfuxueyuan.xyz

[Q73] 查看表状态
来源：http://vka.jinyuanbaomall.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hfv.uphjek.com

[Q74] 强制使用索引
来源：http://ljz.svipenyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vsg.yonumen.top

[Q75] 日期格式化
来源：http://fvg.shanyushiyangtech.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kta.jinyuanbaomall.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hvp.sxryk.cn

[Q76] 按天统计
来源：http://etk.zhixingplan.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dgu.hnxiangtu.top

[Q77] 时间加减
来源：http://fjz.mhx1999.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://phj.chenlongwang.top

[Q78] 当前时间
来源：http://ofh.0kj1m.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fha.yueranfly.top

[Q79] 字符串拼接
来源：http://pfg.zhongyouzk.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jdo.tianlin.xyz

[Q80] 字符串截取
来源：http://zaz.guowangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rzr.quarkkingdee.top

[Q81] 字符串替换
来源：http://xhc.fengsongda.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uqj.wangshuangyany.cn

[Q82] 字符长度与字节长度
来源：http://rqh.ehwqpu.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://isx.jinqigfzy.top

[Q83] 大小写转换
来源：http://zfw.shanyushiyangtech.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gwd.guannengcc.top

[Q84] 去除首尾空格
来源：http://nrz.zdqjudy.top

SELECT TRIM(name) FROM users;
来源：http://zkb.ywan-chungtsiang.top

[Q85] 数值取整
来源：http://aqt.9152youxi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ylr.bbcook.cn

[Q86] 读取 JSON 字段
来源：http://zbq.sysykeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ems.redwolf501.top

[Q87] JSON 字段做条件
来源：http://mur.zhijiandao.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eeg.hfpthk.cn

[Q88] 行转列（条件聚合）
来源：http://lbw.jlsjyb.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://acs.chenjidiqi.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://axu.ybcxt.top

[Q89] 判断表是否存在
来源：http://ysc.guannengcc.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ckp.shanyushiyangtech.top

[Q90] 生成序号列
来源：http://ulx.daxiang520.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mxf.yj202588.top

================================================================================
来源：http://dyi.yongpay.top

R. Bash 专题
来源：http://etr.gotoacloud.top

================================================================================
来源：http://pmq.jiagoushi.top

[R01] shebang 与严格模式
来源：http://wms.ivvv.top

#!/usr/bin/env bash
来源：http://hot.svipenyu.cn

set -euo pipefail
来源：http://lhd.yfazqb.com

[R02] 变量赋值与使用
来源：http://jbf.cucudq.cn

name="Tom"; echo "$name"
来源：http://wbi.zycfv.cn

[R03] 只读变量
来源：http://vnd.ydzc1.top

readonly PI=3.14
来源：http://ucv.ctjpmb.com

[R04] 位置参数
来源：http://oil.hongshengwenyu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qco.tian-w.cn

[R05] 参数默认值
来源：http://lqz.cqqwz.cn

name="${1:-default}"
来源：http://yvz.daxiang520.top

[R06] 判断命令是否存在
来源：http://uhp.cashguo.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qxz.gzhubu.top

[R07] if 判断文件
来源：http://ahz.cashguo.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sef.cheryme.top

[R08] 数值比较
来源：http://jtz.sxryk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://led.cheryme.top

[R09] 字符串比较
来源：http://suc.0kj1m.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://slb.epnwcf.com

[R10] 正则匹配
来源：http://yoh.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://amd.jianghu66.top

[R11] case 多分支
来源：http://tah.gaohongyu789.top

case "$1" in
来源：http://gbf.c1oappe.top

start) echo "启动" ;;
来源：http://kos.pengpengdd.cyou

stop)  echo "停止" ;;
来源：http://ahk.jinyuanbaomall.cn

*)     echo "未知命令" ;;
来源：http://tec.fehbvm.com

esac
来源：http://qad.nanxinkj.top

[R12] for 遍历文件
来源：http://gfr.smart0.xyz

for f in *.txt; do echo "$f"; done
来源：http://mfl.fanxiaobao.xyz

[R13] for 计数循环
来源：http://ntj.zdqjudy.top

for i in {1..10}; do echo "$i"; done
来源：http://rlv.daria6918.cn

[R14] C 风格 for
来源：http://acw.ywan-chungtsiang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zfl.zhiwuduotai.top

[R15] while 逐行读文件
来源：http://ffg.birdmap.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wnr.wangdashe.top

[R16] until 等待条件
来源：http://erz.xingfuxueyuan.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ohm.bbcook.cn

[R17] 数组定义与取值
来源：http://djt.mhx1999.top

arr=(a b c); echo "${arr[0]}"
来源：http://top.52xcode.cn

[R18] 遍历数组
来源：http://juq.tian-w.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wih.aizwys.cn

[R19] 数组长度
来源：http://wwf.sufxvd.cn

echo "${#arr[@]}"
来源：http://ifc.jinqigfzy.top

[R20] 关联数组（字典）
来源：http://twl.9152youxi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://imu.zhijiandao.cn

[R21] 字符串长度
来源：http://hsg.snrcjt.cn

echo "${#s}"
来源：http://qpj.haohaochexian.top

[R22] 截取子串
来源：http://ssg.yanxiufei.cn

echo "${s:0:5}"
来源：http://epk.snrcjt.cn

[R23] 字符串替换
来源：http://xrq.uphjek.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gun.0kj1m.cn

[R24] 大小写转换
来源：http://pbo.haohaochexian.top

echo "${s^^}"; echo "${s,,}"
来源：http://knq.xylfe.cn

[R25] 去后缀 / 去前缀
来源：http://amq.vehdjk.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://nmf.yanxiufei.cn

[R26] 命令替换
来源：http://ext.sweek.top

now=$(date +%F); echo "$now"
来源：http://ijl.sxryk.cn

[R27] 算术展开
来源：http://pdj.hcnkem.com

echo $((1 + 2 * 3))
来源：http://woq.hfpthk.cn

[R28] 浮点运算
来源：http://zza.chenzaomai.com

echo "scale=2; 10/3" | bc
来源：http://yis.hammf.cn

[R29] 定义函数
来源：http://ole.ctjpmb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dnq.kuanghao11.cn

[R30] 函数返回状态码
来源：http://wdi.ivvv.top

f() { return 0; }; f || echo "失败了"
来源：http://yzs.zhixingplan.top

[R31] 局部变量
来源：http://gbc.yanxiufei.cn

f() { local x=1; echo "$x"; }
来源：http://xmb.9152youxi.cn

[R32] 参数个数校验
来源：http://jsz.fktsv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gwa.ppjwa.cn

[R33] 捕获错误并提示行号
来源：http://amf.tianlin.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ezl.zhijiandao.cn

[R34] 退出时清理
来源：http://iyd.zhiwuduotai.top

trap 'rm -f "$tmp"' EXIT
来源：http://ysk.chenzaomai.com

[R35] 后台执行并等待
来源：http://wnq.yongpay.top

sleep 5 & pid=$!; wait "$pid"
来源：http://oct.fengsongda.top

[R36] 并发执行多个任务
来源：http://lmx.52xcode.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sps.nanxinkj.top

[R37] 把输出赋给变量
来源：http://vas.zhijiandao.cn

files=$(ls -1)
来源：http://tbb.cashguo.top

[R38] 管道串联
来源：http://qto.hnxiangtu.top

cat a.txt | grep -i error | wc -l
来源：http://rpb.shzxlz.cn

[R39] 重定向标准输出与错误
来源：http://pzi.zdqjudy.top

cmd > out.log 2>&1
来源：http://nbm.daria6918.cn

[R40] 追加写日志
来源：http://ueb.kuanghao11.cn

echo "log" >> out.log
来源：http://woa.quarkkingdee.top

[R41] 丢弃输出
来源：http://axw.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://rwa.redwolf501.top

[R42] 输入重定向
来源：http://ath.jyoumei.cn

wc -l < a.txt
来源：http://pkp.gzhubu.top

[R43] 按名字查找文件
来源：http://zdo.svipenyu.cn

find . -name "*.log" -type f
来源：http://cpf.iojbl.cn

[R44] 按修改时间查找
来源：http://udu.hongshengwenyu.top

find . -mtime -7 -type f
来源：http://lcw.uphjek.com

[R45] 批量删除
来源：http://fxd.vehdjk.com

find . -name "*.tmp" -delete
来源：http://lde.cucudq.cn

[R46] 递归替换文件内容
来源：http://vnl.zhongyouzk.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uxh.52xcode.cn

[R47] sed 单行替换
来源：http://dvi.hysaishi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://glg.316326.xyz

[R48] awk 取指定列
来源：http://pjk.mhx1999.top

awk '{print $1, $3}' a.txt
来源：http://uam.tanke756.top

[R49] awk 带条件
来源：http://hyc.yueranfly.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yma.yongpay.top

[R50] awk 求和
来源：http://qsx.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://xbf.cdnleiting.top

[R51] 排序去重取前几
来源：http://rwp.fktsv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qfo.jqgfzy.top

[R52] 统计行数
来源：http://rpd.shangyingyoupin.top

wc -l a.txt
来源：http://wqa.bbcook.cn

[R53] 查看文件头与实时尾
来源：http://uvz.jinqigfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jgy.tanke756.top

[R54] 比较两个文件
来源：http://dol.cqqwz.cn

diff a.txt b.txt
来源：http://sev.dianchejie.cn

[R55] 压缩与解压
来源：http://hbt.gaohongyu789.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gtg.ydjk.org.cn

[R56] 远程拷贝
来源：http://vda.guowangkeji.top

scp file user@host:/path/
来源：http://fwx.cheryme.top

[R57] 远程执行命令
来源：http://rfn.tian-w.cn

ssh user@host 'uptime'
来源：http://nzv.feifeiyinyue.top

[R58] 下载文件
来源：http://qjt.nwbrower.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xwy.ydjk.org.cn

[R59] 发 POST JSON
来源：http://tln.havefunace.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fij.jqgufenzy.top

[R60] 只看 HTTP 状态码
来源：http://wfk.meibo888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kgd.zhengqikj.top

[R61] 磁盘占用
来源：http://aeo.kuanghao11.cn

df -h;  du -sh *
来源：http://pzw.jinqigfzy.top

[R62] 找最占空间的文件
来源：http://cqy.zhaomingkeji.xyz

du -ah . | sort -rh | head -10
来源：http://ext.zycfv.cn

[R63] 内存与进程
来源：http://vgv.jiagoushi.top

free -h;  ps aux | grep nginx
来源：http://qzt.sufxvd.cn

[R64] 结束进程
来源：http://duq.hnqzz.top

kill -9 $(pgrep -f app.py)
来源：http://efs.zhengqikj.top

[R65] 查看端口占用
来源：http://yot.0kj1m.cn


<!-- 参考信息 -->