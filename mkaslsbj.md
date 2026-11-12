代发 wailian999

SELECT * FROM users;
来源：http://vxm.ppjwa.cn

[Q16] 查询指定列
来源：http://gda.jinqigufen.top

SELECT id, name FROM users;
来源：http://qjs.gaohongyu789.top

[Q17] 条件查询
来源：http://lwv.dashuyun.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lza.jyoumei.cn

[Q18] 模糊匹配
来源：http://hti.zhixingplan.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xyp.cheryme.top

[Q19] 范围查询
来源：http://uzc.vqdsnc.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gyw.gogol.net.cn

[Q20] IN 列表
来源：http://oqr.ctjpmb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bxy.yueranfly.top

[Q21] 空值判断
来源：http://ogg.daria6918.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qls.hysaishi.cn

[Q22] 排序
来源：http://yps.wangshuangyany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mym.ybcxt.top

[Q23] 分页
来源：http://uhq.cdnleiting.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zkz.xylfe.cn

[Q24] 去重
来源：http://kvi.hfpthk.cn

SELECT DISTINCT city FROM users;
来源：http://for.gaohongyu789.top

[Q25] 只取前 N 条
来源：http://gxs.epnwcf.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://src.aibaodan.cn

[Q26] 计数
来源：http://hhv.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://ams.ivvv.top

[Q27] 条件计数
来源：http://tqe.zhoulong.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fmq.bjfxy.top

[Q28] 求和与平均
来源：http://uey.jqgfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oaa.fanxiaobao.xyz

[Q29] 最大最小值
来源：http://nzj.yueranfly.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gwc.cdnleiting.top

[Q30] 分组统计
来源：http://duj.ywan-chungtsiang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ekp.pengpengdd.cyou

[Q31] 分组后过滤
来源：http://ogf.mhx1999.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kjy.ctjpmb.com

[Q32] 分组拼接字符串
来源：http://ius.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lxo.chenjidiqi.icu

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rch.hongshengwenyu.top

[Q33] 多列分组
来源：http://etx.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uqp.meibo888.top

[Q34] 每组取第一条
来源：http://yyo.316326.xyz

SELECT * FROM (
来源：http://mxl.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sqd.andypj.xyz

) t WHERE rn = 1;
来源：http://lfi.316326.xyz

[Q35] 内连接
来源：http://vcn.redwolf501.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wrf.chenlongwang.top

[Q36] 左连接
来源：http://cwx.jianghu66.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yzr.yonumen.top

[Q37] 右连接
来源：http://oll.yj20258.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://olm.svipenyu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fod.xylfe.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cqy.jinqigufen.top

[Q39] 自连接（查上下级）
来源：http://hlp.vehdjk.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://dbs.zdbjq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xru.hnxiangtu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ttv.xziqi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gun.xinyue.icu

[Q41] 多表连接
来源：http://jhq.zhiwuduotai.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://kvv.kuanghao11.cn

JOIN users u ON u.id = o.user_id
来源：http://avv.zhongyouzk.top

JOIN products p ON p.id = o.product_id;
来源：http://pdr.ywan-chungtsiang.top

[Q42] 连接条件附加过滤
来源：http://kkh.jqgfzy.top

SELECT u.name, o.amount FROM users u
来源：http://mlf.cheryme.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wkj.zdbjq.cn

[Q43] 标量子查询
来源：http://zyl.aibaodan.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xws.feifeiyinyue.top

[Q44] IN 子查询
来源：http://omu.52xcode.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ceb.sxryk.cn

[Q45] EXISTS 判断存在
来源：http://nkg.gogol.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vwp.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xae.gaohongyu789.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mxg.aibaodan.cn

[Q47] 与平均值比较
来源：http://zun.ivvv.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cbl.havefunace.top

[Q48] CTE 公用表表达式
来源：http://kem.zhiwuduotai.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fba.yongpay.top

SELECT * FROM t WHERE c > 5;
来源：http://flv.cdnleiting.top

[Q49] 更新单行
来源：http://oxn.yuxming.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://luu.zycfv.cn

[Q50] 批量更新
来源：http://ybk.hfpthk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pep.hfpthk.cn

[Q51] 用子查询更新
来源：http://gof.dianchejie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dmt.zdqjudy.top

[Q52] 删除指定行
来源：http://efs.xuetiantiany.cn

DELETE FROM users WHERE id = 10;
来源：http://eyy.pengpengdd.cyou

[Q53] 按条件删除
来源：http://kir.gogol.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pbz.jqgfzy.top

[Q54] 清空表
来源：http://hpc.yuanzhike.top

TRUNCATE TABLE logs;
来源：http://ccf.tarul.cn

[Q55] 排名（并列占位）
来源：http://cib.daria6918.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dau.c1oappe.top

[Q56] 密集排名（并列不占位）
来源：http://czk.xziqi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cpj.zhixingplan.top

[Q57] 行号
来源：http://iei.gzhubu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gjf.yuxming.cn

[Q58] 累计求和
来源：http://emn.316326.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eng.snrcjt.cn

[Q59] 分组内累计
来源：http://bgd.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bfq.epnwcf.com

[Q60] 取上一行 / 下一行
来源：http://efk.shanyushiyangkeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bwq.yuanzhike.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ktd.xingfuxueyuan.xyz

[Q61] 移动平均
来源：http://nli.guannengcc.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fmf.yangfankeji.com

[Q62] 分组占比
来源：http://qgl.shanyushiyangkeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oxz.jinghuilouyu.cn

[Q63] 开启事务
来源：http://gjr.cqqwz.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://naz.andypj.xyz

[Q64] 提交事务
来源：http://syx.havefunace.top

COMMIT;
来源：http://bun.hesvh.cn

[Q65] 回滚事务
来源：http://xwk.hammf.cn

ROLLBACK;
来源：http://xlg.yangfankeji.com

[Q66] 行锁查询
来源：http://epx.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://chq.dashuyun.cn

[Q67] 设置隔离级别
来源：http://npg.yj202588.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rta.ywan-chungtsiang.top

[Q68] 保存点
来源：http://jid.shanyushiyangkeji.top

SAVEPOINT sp1;
来源：http://zlf.sjlbkw.cn

ROLLBACK TO sp1;
来源：http://lnf.fengsongda.top

[Q69] 查看执行计划
来源：http://dfo.fehbvm.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bru.aizwys.cn

[Q70] 更新统计信息
来源：http://tvv.dianchejie.cn

ANALYZE TABLE users;
来源：http://dkm.yongpay.top

[Q71] 查看建表语句
来源：http://irc.jiagoushi.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bxe.gzhubu.top

[Q72] 查看索引
来源：http://ubx.gotoacloud.top

SHOW INDEX FROM users;
来源：http://ytc.meibo888.top

[Q73] 查看表状态
来源：http://jhw.zycfv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fyn.shuidangran.top

[Q74] 强制使用索引
来源：http://cfu.52xcode.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://evf.tarul.cn

[Q75] 日期格式化
来源：http://eid.cheryme.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mht.fehbvm.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qdy.9152youxi.cn

[Q76] 按天统计
来源：http://ymy.uphjek.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kep.fanxiaobao.xyz

[Q77] 时间加减
来源：http://mco.fzhhl.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://llq.vqdsnc.cn

[Q78] 当前时间
来源：http://kxc.gaohongyu789.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cme.hcnkem.com

[Q79] 字符串拼接
来源：http://xse.yj202588.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://byv.316326.xyz

[Q80] 字符串截取
来源：http://sly.bbcook.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lla.yueranfly.top

[Q81] 字符串替换
来源：http://izp.zhiwuduotai.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uvp.bjfxy.top

[Q82] 字符长度与字节长度
来源：http://rjt.quarkkingdee.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vsc.yfazqb.com

[Q83] 大小写转换
来源：http://hpf.hammf.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gdg.shanyushiyangkeji.top

[Q84] 去除首尾空格
来源：http://qco.hnqzz.top

SELECT TRIM(name) FROM users;
来源：http://sme.chenzaomai.com

[Q85] 数值取整
来源：http://pma.guannengcc.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://foy.svipenyu.cn

[Q86] 读取 JSON 字段
来源：http://vxm.chenlongwang.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gih.52xcode.cn

[Q87] JSON 字段做条件
来源：http://yke.epnwcf.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://biu.feifeiyinyue.top

[Q88] 行转列（条件聚合）
来源：http://gjd.cashguo.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dxz.gzhubu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sat.gotoacloud.top

[Q89] 判断表是否存在
来源：http://dkq.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mbm.pycfn.com

[Q90] 生成序号列
来源：http://akf.xuetiantiany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mrm.yj202588.top

================================================================================
来源：http://rhq.shanyushiyangkeji.top

R. Bash 专题
来源：http://jvw.jqgfzy.top

================================================================================
来源：http://xfm.hongshengwenyu.top

[R01] shebang 与严格模式
来源：http://evq.pycfn.com

#!/usr/bin/env bash
来源：http://lve.jinqigufen.top

set -euo pipefail
来源：http://yuw.hfpthk.cn

[R02] 变量赋值与使用
来源：http://clm.yueranfly.top

name="Tom"; echo "$name"
来源：http://rbh.cdnleiting.top

[R03] 只读变量
来源：http://cut.yuxming.cn

readonly PI=3.14
来源：http://qpw.ydzc1.top

[R04] 位置参数
来源：http://shc.pycfn.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://euk.316326.xyz

[R05] 参数默认值
来源：http://ksf.snrcjt.cn

name="${1:-default}"
来源：http://mya.yj20258888.top

[R06] 判断命令是否存在
来源：http://kjw.jiagoushi.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rgi.sufxvd.cn

[R07] if 判断文件
来源：http://clo.hywenlv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kpd.52xcode.cn

[R08] 数值比较
来源：http://spl.tarul.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uyi.yvedp.cn

[R09] 字符串比较
来源：http://dxu.yongpay.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dqh.pycfn.com

[R10] 正则匹配
来源：http://jfk.nanxinkj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://epz.zhoulong.xyz

[R11] case 多分支
来源：http://bnk.aizwys.cn

case "$1" in
来源：http://mzu.shanyushiyangkeji.top

start) echo "启动" ;;
来源：http://kfu.nanxinkj.top

stop)  echo "停止" ;;
来源：http://fdz.yj20258.top

*)     echo "未知命令" ;;
来源：http://vup.cheryme.top

esac
来源：http://npb.meibo888.top

[R12] for 遍历文件
来源：http://tyn.jyoumei.cn

for f in *.txt; do echo "$f"; done
来源：http://qut.haohaochexian.top

[R13] for 计数循环
来源：http://wlt.c1oappe.top

for i in {1..10}; do echo "$i"; done
来源：http://bfq.tian-w.cn

[R14] C 风格 for
来源：http://wcn.havefunace.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lhk.andypj.xyz

[R15] while 逐行读文件
来源：http://olb.yonumen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nls.jiagoushi.top

[R16] until 等待条件
来源：http://bwn.yvedp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kpu.dashuyun.cn

[R17] 数组定义与取值
来源：http://mcv.hfpthk.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rju.pengpengdd.cyou

[R18] 遍历数组
来源：http://wbq.guowangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hxy.fktsv.cn

[R19] 数组长度
来源：http://fsw.yanxiufei.cn

echo "${#arr[@]}"
来源：http://jhs.dianchejie.cn

[R20] 关联数组（字典）
来源：http://uqc.hnqzz.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://asw.shzxlz.cn

[R21] 字符串长度
来源：http://wfz.sxryk.cn

echo "${#s}"
来源：http://vsf.zycfv.cn

[R22] 截取子串
来源：http://zfz.nwbrower.top

echo "${s:0:5}"
来源：http://sxn.jqgfzy.top

[R23] 字符串替换
来源：http://lfz.ywan-chungtsiang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pzh.ehwqpu.com

[R24] 大小写转换
来源：http://gnx.ydjk.org.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gho.zhixingplan.top

[R25] 去后缀 / 去前缀
来源：http://zgp.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nzi.gotoacloud.top

[R26] 命令替换
来源：http://cwn.yfazqb.com

now=$(date +%F); echo "$now"
来源：http://hrs.mhx1999.top

[R27] 算术展开
来源：http://bsu.zdbjq.cn

echo $((1 + 2 * 3))
来源：http://svh.hesvh.cn

[R28] 浮点运算
来源：http://hnd.jianghu66.top

echo "scale=2; 10/3" | bc
来源：http://viu.xuanzx.com

[R29] 定义函数
来源：http://cee.birdmap.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eqr.zhaomingkeji.xyz

[R30] 函数返回状态码
来源：http://vjn.haohaochexian.top

f() { return 0; }; f || echo "失败了"
来源：http://qud.cdnleiting.top

[R31] 局部变量
来源：http://bjr.snrcjt.cn

f() { local x=1; echo "$x"; }
来源：http://stx.jinyuanbaomall.cn

[R32] 参数个数校验
来源：http://gga.zdbjq.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tnm.jinghuilouyu.cn

[R33] 捕获错误并提示行号
来源：http://rkt.jqgfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kse.hesvh.cn

[R34] 退出时清理
来源：http://zfj.ydzc1.top

trap 'rm -f "$tmp"' EXIT
来源：http://oms.ydjk.org.cn

[R35] 后台执行并等待
来源：http://xfh.birdmap.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xot.zycfv.cn

[R36] 并发执行多个任务
来源：http://xub.jqgufenzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://woi.hammf.cn

[R37] 把输出赋给变量
来源：http://wgi.feifeiyinyue.top

files=$(ls -1)
来源：http://lce.jianghu66.top

[R38] 管道串联
来源：http://igf.sjlbkw.cn

cat a.txt | grep -i error | wc -l
来源：http://pop.chenjidiqi.icu

[R39] 重定向标准输出与错误
来源：http://byy.zdbjq.cn

cmd > out.log 2>&1
来源：http://yyr.jqgfzy.top

[R40] 追加写日志
来源：http://sho.epnwcf.com

echo "log" >> out.log
来源：http://lai.snrcjt.cn

[R41] 丢弃输出
来源：http://zkz.yfazqb.com

cmd >/dev/null 2>&1
来源：http://jgy.epnwcf.com

[R42] 输入重定向
来源：http://glk.daria6918.cn

wc -l < a.txt
来源：http://hzf.fanxiaobao.xyz

[R43] 按名字查找文件
来源：http://nst.nanxinkj.top

find . -name "*.log" -type f
来源：http://zqd.ydjk.org.cn

[R44] 按修改时间查找
来源：http://zjt.aibaodan.cn

find . -mtime -7 -type f
来源：http://drw.sjlbkw.cn

[R45] 批量删除
来源：http://fkh.smart0.xyz

find . -name "*.tmp" -delete
来源：http://pel.yangfankeji.com

[R46] 递归替换文件内容
来源：http://vnd.ydjk.org.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sko.chenzaomai.com

[R47] sed 单行替换
来源：http://eup.zhijiandao.cn

sed -i 's/foo/bar/g' a.txt
来源：http://eph.yonumen.top

[R48] awk 取指定列
来源：http://tfw.yj202588.top

awk '{print $1, $3}' a.txt
来源：http://ioy.snrcjt.cn

[R49] awk 带条件
来源：http://bjk.dashuyun.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yus.cucudq.cn

[R50] awk 求和
来源：http://hjw.zhijiandao.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bhp.yongpay.top

[R51] 排序去重取前几
来源：http://htq.cheryme.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gip.cheryme.top

[R52] 统计行数
来源：http://srq.ybcxt.top

wc -l a.txt
来源：http://jet.xinyue.icu

[R53] 查看文件头与实时尾
来源：http://nlp.jlsjyb.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://imx.zhongyouzk.top

[R54] 比较两个文件
来源：http://qav.yongpay.top

diff a.txt b.txt
来源：http://ksu.hysaishi.cn

[R55] 压缩与解压
来源：http://eal.tarul.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://afg.hywenlv.cn

[R56] 远程拷贝
来源：http://eqg.sjlbkw.cn

scp file user@host:/path/
来源：http://ywa.ydjk.org.cn

[R57] 远程执行命令
来源：http://quz.guannengcc.top

ssh user@host 'uptime'
来源：http://asu.pycfn.com

[R58] 下载文件
来源：http://xvp.ywan-chungtsiang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yds.jiagoushi.top

[R59] 发 POST JSON
来源：http://fsa.nanxuanxn.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://btw.ppjwa.cn

[R60] 只看 HTTP 状态码
来源：http://kvy.xylfe.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rxr.c1oappe.top

[R61] 磁盘占用
来源：http://yqb.gzhubu.top

df -h;  du -sh *
来源：http://vqj.gotoacloud.top

[R62] 找最占空间的文件
来源：http://ufx.pengpengdd.cyou

du -ah . | sort -rh | head -10
来源：http://jiz.9152youxi.cn

[R63] 内存与进程
来源：http://thi.haohaochexian.top

free -h;  ps aux | grep nginx
来源：http://vzt.sjlbkw.cn

[R64] 结束进程
来源：http://qaf.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://uma.svipenyu.cn

[R65] 查看端口占用
来源：http://hss.epnwcf.com


<!-- 参考信息 -->