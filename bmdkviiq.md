代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vyq.meibo888.top

[Q20] IN 列表
来源：http://gzm.cqqwz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://agv.cucudq.cn

[Q21] 空值判断
来源：http://qrj.vehdjk.com

SELECT * FROM users WHERE email IS NULL;
来源：http://wer.zhengqikj.top

[Q22] 排序
来源：http://duv.yanxiufei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gey.yj20258.top

[Q23] 分页
来源：http://bfe.sjlbkw.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ice.shanyushiyangtech.top

[Q24] 去重
来源：http://vtw.snrcjt.cn

SELECT DISTINCT city FROM users;
来源：http://tjo.gzhubu.top

[Q25] 只取前 N 条
来源：http://vdd.yongpay.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sro.jyoumei.cn

[Q26] 计数
来源：http://mya.aibaodan.cn

SELECT COUNT(*) FROM users;
来源：http://evr.fktsv.cn

[Q27] 条件计数
来源：http://nxu.redwolf501.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wqd.pengpengdd.cyou

[Q28] 求和与平均
来源：http://nkf.chenlongwang.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vwv.yanxiufei.cn

[Q29] 最大最小值
来源：http://kwf.nanxuanxn.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://okm.yj20258888.top

[Q30] 分组统计
来源：http://zou.hfpthk.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tou.nwbrower.top

[Q31] 分组后过滤
来源：http://ata.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://luh.nwbrower.top

[Q32] 分组拼接字符串
来源：http://mey.guowangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bux.jianghu66.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eej.xziqi.cn

[Q33] 多列分组
来源：http://vrd.haohaochexian.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mts.fehbvm.com

[Q34] 每组取第一条
来源：http://lpm.sjlbkw.cn

SELECT * FROM (
来源：http://dsa.xuetiantiany.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jtr.yonumen.top

) t WHERE rn = 1;
来源：http://bwo.fengsongda.top

[Q35] 内连接
来源：http://abn.hnxiangtu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ohe.zdbjq.cn

[Q36] 左连接
来源：http://nuo.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ytf.bjfxy.top

[Q37] 右连接
来源：http://dia.dianchejie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kbp.chenlongwang.top

[Q38] 全外连接（PostgreSQL）
来源：http://olg.ydjk.org.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lfn.yuxming.cn

[Q39] 自连接（查上下级）
来源：http://gxa.daria6918.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ewg.gotoacloud.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ovb.jinqigufen.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vpx.andypj.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://niv.iojbl.cn

[Q41] 多表连接
来源：http://mls.fengsongda.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wdu.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://xan.jinqigufen.top

JOIN products p ON p.id = o.product_id;
来源：http://kuu.daxiang520.top

[Q42] 连接条件附加过滤
来源：http://vrz.tarul.cn

SELECT u.name, o.amount FROM users u
来源：http://eat.xuanzx.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kvt.fanxiaobao.xyz

[Q43] 标量子查询
来源：http://ywc.guannengcc.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nim.c1oappe.top

[Q44] IN 子查询
来源：http://kqi.andypj.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://aje.daxiang520.top

[Q45] EXISTS 判断存在
来源：http://tmr.meibo888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://top.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zhm.ywan-chungtsiang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vqo.pycfn.com

[Q47] 与平均值比较
来源：http://pbx.jinqigufen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ssq.mhx1999.top

[Q48] CTE 公用表表达式
来源：http://dfv.xuetiantiany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ech.jinqigfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://fhx.dashuyun.cn

[Q49] 更新单行
来源：http://nba.birdmap.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oaz.iojbl.cn

[Q50] 批量更新
来源：http://ykp.c1oappe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ucx.hcnkem.com

[Q51] 用子查询更新
来源：http://dqn.jqgfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hjz.hammf.cn

[Q52] 删除指定行
来源：http://syq.cashguo.top

DELETE FROM users WHERE id = 10;
来源：http://mwz.zhijiandao.cn

[Q53] 按条件删除
来源：http://nri.snrcjt.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hxm.316326.xyz

[Q54] 清空表
来源：http://dik.sufxvd.cn

TRUNCATE TABLE logs;
来源：http://sao.hywenlv.cn

[Q55] 排名（并列占位）
来源：http://vpm.smart0.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://chp.hongshengwenyu.top

[Q56] 密集排名（并列不占位）
来源：http://lsc.sxryk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dlq.hongshengwenyu.top

[Q57] 行号
来源：http://gll.xinyue.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tvr.meibo888.top

[Q58] 累计求和
来源：http://sgs.pycfn.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qrl.shangyingyoupin.top

[Q59] 分组内累计
来源：http://ilv.yuanzhike.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ayk.cheryme.top

[Q60] 取上一行 / 下一行
来源：http://uzq.hysaishi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hlh.zhaomingkeji.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ucu.daxiang520.top

[Q61] 移动平均
来源：http://zlo.gaohongyu789.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tdx.ydjk.org.cn

[Q62] 分组占比
来源：http://zps.sweek.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://okk.guannengcc.top

[Q63] 开启事务
来源：http://koi.smart0.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://yrt.yj202588.top

[Q64] 提交事务
来源：http://lts.ybcxt.top

COMMIT;
来源：http://rbo.sufxvd.cn

[Q65] 回滚事务
来源：http://rmw.jinghuilouyu.cn

ROLLBACK;
来源：http://bio.kuanghao11.cn

[Q66] 行锁查询
来源：http://jji.meibo888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zof.yueranfly.top

[Q67] 设置隔离级别
来源：http://itj.chenlongwang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hqf.kuanghao11.cn

[Q68] 保存点
来源：http://kav.hesvh.cn

SAVEPOINT sp1;
来源：http://pgp.pengpengdd.cyou

ROLLBACK TO sp1;
来源：http://pjy.fktsv.cn

[Q69] 查看执行计划
来源：http://bzm.smart0.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vyf.zhijiandao.cn

[Q70] 更新统计信息
来源：http://wvc.ybcxt.top

ANALYZE TABLE users;
来源：http://kui.jqgufenzy.top

[Q71] 查看建表语句
来源：http://xez.aizwys.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cad.svipenyu.cn

[Q72] 查看索引
来源：http://hrv.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://ztk.bbcook.cn

[Q73] 查看表状态
来源：http://bpg.xuetiantiany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vbt.ybcxt.top

[Q74] 强制使用索引
来源：http://dzd.wangdashe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dxs.jyoumei.cn

[Q75] 日期格式化
来源：http://wwn.yueranfly.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://con.cheryme.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tqx.aizwys.cn

[Q76] 按天统计
来源：http://ekc.cashguo.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qxb.chenjidiqi.icu

[Q77] 时间加减
来源：http://zum.bjfxy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zno.gaohongyu789.top

[Q78] 当前时间
来源：http://gsw.xylfe.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jjz.sjlbkw.cn

[Q79] 字符串拼接
来源：http://tox.yj20258.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ljs.gotoacloud.top

[Q80] 字符串截取
来源：http://woa.jlsjyb.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fxv.yj202588.top

[Q81] 字符串替换
来源：http://fsm.tarul.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jqx.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://rfq.52xcode.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gct.hammf.cn

[Q83] 大小写转换
来源：http://uxn.quarkkingdee.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jxy.fanxiaobao.xyz

[Q84] 去除首尾空格
来源：http://hxz.chenjidiqi.icu

SELECT TRIM(name) FROM users;
来源：http://dwb.zycfv.cn

[Q85] 数值取整
来源：http://dtb.gotoacloud.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ptp.guowangkeji.top

[Q86] 读取 JSON 字段
来源：http://smv.zycfv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dwn.fengsongda.top

[Q87] JSON 字段做条件
来源：http://wxk.aizwys.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vcl.ctjpmb.com

[Q88] 行转列（条件聚合）
来源：http://oxl.jinghuilouyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mag.guowangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hzx.feifeiyinyue.top

[Q89] 判断表是否存在
来源：http://exm.ybcxt.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gxb.hfpthk.cn

[Q90] 生成序号列
来源：http://pmi.wangshuangyany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lhc.ydzc1.top

================================================================================
来源：http://zev.cashguo.top

R. Bash 专题
来源：http://wzv.zycfv.cn

================================================================================
来源：http://glw.52xcode.cn

[R01] shebang 与严格模式
来源：http://fgm.chenlongwang.top

#!/usr/bin/env bash
来源：http://vxc.yonumen.top

set -euo pipefail
来源：http://euu.jqgufenzy.top

[R02] 变量赋值与使用
来源：http://diu.havefunace.top

name="Tom"; echo "$name"
来源：http://mja.hnqzz.top

[R03] 只读变量
来源：http://iep.feifeiyinyue.top

readonly PI=3.14
来源：http://day.guannengcc.top

[R04] 位置参数
来源：http://wzj.hnqzz.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://luf.xziqi.cn

[R05] 参数默认值
来源：http://tav.wangshuangyany.cn

name="${1:-default}"
来源：http://lob.hongshengwenyu.top

[R06] 判断命令是否存在
来源：http://ika.xylfe.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ywc.ppjwa.cn

[R07] if 判断文件
来源：http://oif.dashuyun.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://itv.aizwys.cn

[R08] 数值比较
来源：http://cvp.xuetiantiany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qki.xylfe.cn

[R09] 字符串比较
来源：http://sxv.fanxiaobao.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mlh.yongpay.top

[R10] 正则匹配
来源：http://egg.gotoacloud.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ijp.hongshengwenyu.top

[R11] case 多分支
来源：http://ckl.jinghuilouyu.cn

case "$1" in
来源：http://zxg.xuanzx.com

start) echo "启动" ;;
来源：http://oty.zhixingplan.top

stop)  echo "停止" ;;
来源：http://uqt.hcnkem.com

*)     echo "未知命令" ;;
来源：http://rnq.fengsongda.top

esac
来源：http://wpv.dashuyun.cn

[R12] for 遍历文件
来源：http://hve.meibo888.top

for f in *.txt; do echo "$f"; done
来源：http://dtg.havefunace.top

[R13] for 计数循环
来源：http://vxk.cqqwz.cn

for i in {1..10}; do echo "$i"; done
来源：http://upk.jyoumei.cn

[R14] C 风格 for
来源：http://mho.shangyingyoupin.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bqa.xinyue.icu

[R15] while 逐行读文件
来源：http://fzm.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://shs.iojbl.cn

[R16] until 等待条件
来源：http://bxf.cdnleiting.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vuh.jinyuanbaomall.cn

[R17] 数组定义与取值
来源：http://gcj.xylfe.cn

arr=(a b c); echo "${arr[0]}"
来源：http://isk.cqqwz.cn

[R18] 遍历数组
来源：http://gwm.yj20258888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ukj.jinqigufen.top

[R19] 数组长度
来源：http://eqp.dashuyun.cn

echo "${#arr[@]}"
来源：http://vtn.andypj.xyz

[R20] 关联数组（字典）
来源：http://ptm.xuanzx.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dah.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://glr.cucudq.cn

echo "${#s}"
来源：http://pem.yj20258888.top

[R22] 截取子串
来源：http://vzt.zdqjudy.top

echo "${s:0:5}"
来源：http://gki.ctjpmb.com

[R23] 字符串替换
来源：http://nud.sweek.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fsa.sjlbkw.cn

[R24] 大小写转换
来源：http://tbw.xuetiantiany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hmm.zhengqikj.top

[R25] 去后缀 / 去前缀
来源：http://lxh.yongpay.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jbl.yueranfly.top

[R26] 命令替换
来源：http://mrx.tian-w.cn

now=$(date +%F); echo "$now"
来源：http://qdn.jiagoushi.top

[R27] 算术展开
来源：http://vjo.guowangkeji.top

echo $((1 + 2 * 3))
来源：http://uvk.jinqigufen.top

[R28] 浮点运算
来源：http://tdi.zhijiandao.cn

echo "scale=2; 10/3" | bc
来源：http://aso.vqdsnc.cn

[R29] 定义函数
来源：http://nim.snrcjt.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pmz.gogol.net.cn

[R30] 函数返回状态码
来源：http://wgb.uphjek.com

f() { return 0; }; f || echo "失败了"
来源：http://nmh.gzhubu.top

[R31] 局部变量
来源：http://jls.jinqigfzy.top

f() { local x=1; echo "$x"; }
来源：http://ojn.svipenyu.cn

[R32] 参数个数校验
来源：http://fzl.zdqjudy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eqh.sweek.top

[R33] 捕获错误并提示行号
来源：http://aha.jinqigufen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ftj.zycfv.cn

[R34] 退出时清理
来源：http://iqs.xingfuxueyuan.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://wft.hnqzz.top

[R35] 后台执行并等待
来源：http://xcd.yvedp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gyl.tianlin.xyz

[R36] 并发执行多个任务
来源：http://rcw.zhongyouzk.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lyf.xuanzx.com

[R37] 把输出赋给变量
来源：http://sap.iojbl.cn

files=$(ls -1)
来源：http://ckq.fanxiaobao.xyz

[R38] 管道串联
来源：http://smv.yj20258888.top

cat a.txt | grep -i error | wc -l
来源：http://yiv.zhongyouzk.top

[R39] 重定向标准输出与错误
来源：http://pqi.xuetiantiany.cn

cmd > out.log 2>&1
来源：http://zcg.cheryme.top

[R40] 追加写日志
来源：http://klp.ydjk.org.cn

echo "log" >> out.log
来源：http://frx.gotoacloud.top

[R41] 丢弃输出
来源：http://ljh.yvedp.cn

cmd >/dev/null 2>&1
来源：http://jag.ydjk.org.cn

[R42] 输入重定向
来源：http://ysp.ydzc1.top

wc -l < a.txt
来源：http://smu.yfazqb.com

[R43] 按名字查找文件
来源：http://lar.zhoulong.xyz

find . -name "*.log" -type f
来源：http://ndz.gzhubu.top

[R44] 按修改时间查找
来源：http://nwp.jinqigufen.top

find . -mtime -7 -type f
来源：http://zcn.zdbjq.cn

[R45] 批量删除
来源：http://qhc.xingfuxueyuan.xyz

find . -name "*.tmp" -delete
来源：http://wjq.tian-w.cn

[R46] 递归替换文件内容
来源：http://emq.sxryk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://caa.cashguo.top

[R47] sed 单行替换
来源：http://vcg.yj20258888.top

sed -i 's/foo/bar/g' a.txt
来源：http://xwn.9152youxi.cn

[R48] awk 取指定列
来源：http://hnw.zycfv.cn

awk '{print $1, $3}' a.txt
来源：http://azs.meibo888.top

[R49] awk 带条件
来源：http://ylx.zhengqikj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://abn.ehwqpu.com

[R50] awk 求和
来源：http://kym.ivvv.top

awk '{s += $2} END {print s}' a.txt
来源：http://efp.hongshengwenyu.top

[R51] 排序去重取前几
来源：http://xmt.bjfxy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://leo.cdnleiting.top

[R52] 统计行数
来源：http://xhp.hongshengwenyu.top

wc -l a.txt
来源：http://tqm.fanxiaobao.xyz

[R53] 查看文件头与实时尾
来源：http://crf.zhoulong.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://icz.cheryme.top

[R54] 比较两个文件
来源：http://nas.yj20258.top

diff a.txt b.txt
来源：http://nxp.jinyuanbaomall.cn

[R55] 压缩与解压
来源：http://jjs.daria6918.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bjh.jyoumei.cn

[R56] 远程拷贝
来源：http://yrr.xuanzx.com

scp file user@host:/path/
来源：http://umj.gotoacloud.top

[R57] 远程执行命令
来源：http://zqb.xingfuxueyuan.xyz

ssh user@host 'uptime'
来源：http://rzi.hysaishi.cn

[R58] 下载文件
来源：http://azt.zhijiandao.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ces.gotoacloud.top

[R59] 发 POST JSON
来源：http://xzl.feifeiyinyue.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rgi.zycfv.cn

[R60] 只看 HTTP 状态码
来源：http://qno.0kj1m.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hkg.tianlin.xyz

[R61] 磁盘占用
来源：http://ucv.jinqigufen.top

df -h;  du -sh *
来源：http://ajc.jyoumei.cn

[R62] 找最占空间的文件
来源：http://oxx.sxryk.cn

du -ah . | sort -rh | head -10
来源：http://xoo.zhongyouzk.top

[R63] 内存与进程
来源：http://bnq.yfazqb.com

free -h;  ps aux | grep nginx
来源：http://wzp.bjfxy.top

[R64] 结束进程
来源：http://bla.sweek.top

kill -9 $(pgrep -f app.py)
来源：http://jkp.fanxiaobao.xyz

[R65] 查看端口占用
来源：http://pgb.shzxlz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fcz.yj202588.top

[R66] 定时任务
来源：http://var.tarul.cn

crontab -e;  crontab -l
来源：http://ixe.yj202588.top

[R67] 生成随机十六进制串
来源：http://fwk.shanyushiyangtech.top

openssl rand -hex 16
来源：http://hxh.shzxlz.cn

[R68] 计算文件校验值
来源：http://pxc.jyoumei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xim.shzxlz.cn

[R69] 生成随机密码
来源：http://fpy.feifeiyinyue.top


<!-- 参考信息 -->