代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bxl.hnxiangtu.top

[Q18] 模糊匹配
来源：http://ucc.gogol.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lmb.yonumen.top

[Q19] 范围查询
来源：http://ver.pengpengdd.cyou

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qte.ydjk.org.cn

[Q20] IN 列表
来源：http://oeu.birdmap.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mil.yanxiufei.cn

[Q21] 空值判断
来源：http://uoh.xylfe.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rdn.chenzaomai.com

[Q22] 排序
来源：http://oyw.aibaodan.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://els.haohaochexian.top

[Q23] 分页
来源：http://tte.snrcjt.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ohe.c1oappe.top

[Q24] 去重
来源：http://pkt.gogol.net.cn

SELECT DISTINCT city FROM users;
来源：http://zwa.jqgfzy.top

[Q25] 只取前 N 条
来源：http://ufp.sysykeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://atd.316326.xyz

[Q26] 计数
来源：http://elu.chenzaomai.com

SELECT COUNT(*) FROM users;
来源：http://wcs.ybcxt.top

[Q27] 条件计数
来源：http://shp.ctjpmb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pom.sweek.top

[Q28] 求和与平均
来源：http://psg.feifeiyinyue.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dnj.yj202588.top

[Q29] 最大最小值
来源：http://gcn.c1oappe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yzz.aibaodan.cn

[Q30] 分组统计
来源：http://jop.jqgufenzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rzb.hammf.cn

[Q31] 分组后过滤
来源：http://jju.shuidangran.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wvm.tianlin.xyz

[Q32] 分组拼接字符串
来源：http://bpi.yanxiufei.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://naf.yvedp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ajm.tanke756.top

[Q33] 多列分组
来源：http://dtt.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ybv.jqgfzy.top

[Q34] 每组取第一条
来源：http://tfz.cdnleiting.top

SELECT * FROM (
来源：http://iwr.tianlin.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fbe.gogol.net.cn

) t WHERE rn = 1;
来源：http://mdw.ivvv.top

[Q35] 内连接
来源：http://ugn.jyoumei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uqf.zdqjudy.top

[Q36] 左连接
来源：http://udu.jianghu66.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qwg.yonumen.top

[Q37] 右连接
来源：http://ttb.birdmap.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mgk.zhengqikj.top

[Q38] 全外连接（PostgreSQL）
来源：http://man.tarul.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yia.zhongyouzk.top

[Q39] 自连接（查上下级）
来源：http://xfm.hongshengwenyu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zbu.ywan-chungtsiang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gyb.hesvh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ygj.bjfxy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://owa.shanyushiyangtech.top

[Q41] 多表连接
来源：http://qci.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://iqt.vqdsnc.cn

JOIN users u ON u.id = o.user_id
来源：http://udo.jiagoushi.top

JOIN products p ON p.id = o.product_id;
来源：http://vaw.nwbrower.top

[Q42] 连接条件附加过滤
来源：http://lfn.yonumen.top

SELECT u.name, o.amount FROM users u
来源：http://upm.yanxiufei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://drb.andypj.xyz

[Q43] 标量子查询
来源：http://ijq.dashuyun.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zcg.yanxiufei.cn

[Q44] IN 子查询
来源：http://fwt.dianchejie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tnz.yongpay.top

[Q45] EXISTS 判断存在
来源：http://tmw.ywan-chungtsiang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hhw.sweek.top

[Q46] NOT EXISTS 判断不存在
来源：http://kuj.zdbjq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://htc.9152youxi.cn

[Q47] 与平均值比较
来源：http://zer.fengsongda.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uod.tian-w.cn

[Q48] CTE 公用表表达式
来源：http://lsc.zdbjq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bzo.sxryk.cn

SELECT * FROM t WHERE c > 5;
来源：http://hyj.ydzc1.top

[Q49] 更新单行
来源：http://urx.tarul.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hmf.shuidangran.top

[Q50] 批量更新
来源：http://jnm.jiagoushi.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bpm.fengsongda.top

[Q51] 用子查询更新
来源：http://ndz.hysaishi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zfq.shanyushiyangtech.top

[Q52] 删除指定行
来源：http://frp.cdnleiting.top

DELETE FROM users WHERE id = 10;
来源：http://djn.shuidangran.top

[Q53] 按条件删除
来源：http://urg.ppjwa.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tgn.0kj1m.cn

[Q54] 清空表
来源：http://gby.gzhubu.top

TRUNCATE TABLE logs;
来源：http://rrk.ybcxt.top

[Q55] 排名（并列占位）
来源：http://ysf.316326.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kbp.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://wjg.yvedp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://coc.sxryk.cn

[Q57] 行号
来源：http://flz.tanke756.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://stq.shuidangran.top

[Q58] 累计求和
来源：http://edd.yongpay.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eis.uphjek.com

[Q59] 分组内累计
来源：http://glh.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nuh.sysykeji.top

[Q60] 取上一行 / 下一行
来源：http://mdz.zhoulong.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wiy.0kj1m.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://aqw.mhx1999.top

[Q61] 移动平均
来源：http://yvh.daxiang520.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ohz.zhoulong.xyz

[Q62] 分组占比
来源：http://huq.jyoumei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cho.cashguo.top

[Q63] 开启事务
来源：http://lxw.svipenyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kah.yj20258.top

[Q64] 提交事务
来源：http://rxr.cheryme.top

COMMIT;
来源：http://xul.vehdjk.com

[Q65] 回滚事务
来源：http://tlv.gotoacloud.top

ROLLBACK;
来源：http://eul.ehwqpu.com

[Q66] 行锁查询
来源：http://gin.meibo888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dvl.nwbrower.top

[Q67] 设置隔离级别
来源：http://zxa.zhaomingkeji.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eyy.daria6918.cn

[Q68] 保存点
来源：http://yin.zhixingplan.top

SAVEPOINT sp1;
来源：http://exs.yueranfly.top

ROLLBACK TO sp1;
来源：http://zjn.shuidangran.top

[Q69] 查看执行计划
来源：http://rws.0kj1m.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mfd.redwolf501.top

[Q70] 更新统计信息
来源：http://nuo.fktsv.cn

ANALYZE TABLE users;
来源：http://mul.aizwys.cn

[Q71] 查看建表语句
来源：http://gux.fktsv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qjz.daria6918.cn

[Q72] 查看索引
来源：http://vrm.jinqigufen.top

SHOW INDEX FROM users;
来源：http://czr.tarul.cn

[Q73] 查看表状态
来源：http://cng.gogol.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dcr.daria6918.cn

[Q74] 强制使用索引
来源：http://idn.jqgfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mcf.pengpengdd.cyou

[Q75] 日期格式化
来源：http://epk.iojbl.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pzi.52xcode.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cec.tanke756.top

[Q76] 按天统计
来源：http://fnk.gzhubu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://umk.tianlin.xyz

[Q77] 时间加减
来源：http://blh.zhongyouzk.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ufg.ydzc1.top

[Q78] 当前时间
来源：http://cad.cqqwz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ozd.ivvv.top

[Q79] 字符串拼接
来源：http://rim.shangyingyoupin.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tdc.tanke756.top

[Q80] 字符串截取
来源：http://upo.shanyushiyangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jhy.hammf.cn

[Q81] 字符串替换
来源：http://mlw.ydjk.org.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jbr.epnwcf.com

[Q82] 字符长度与字节长度
来源：http://epp.sysykeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fee.sysykeji.top

[Q83] 大小写转换
来源：http://tci.zycfv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fyq.fanxiaobao.xyz

[Q84] 去除首尾空格
来源：http://tdd.nanxinkj.top

SELECT TRIM(name) FROM users;
来源：http://reo.gzhubu.top

[Q85] 数值取整
来源：http://tca.shanyushiyangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ugt.nwbrower.top

[Q86] 读取 JSON 字段
来源：http://vdl.hfpthk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sxf.fehbvm.com

[Q87] JSON 字段做条件
来源：http://vjv.gogol.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://upw.shanyushiyangkeji.top

[Q88] 行转列（条件聚合）
来源：http://geg.sxryk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lql.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nzh.haohaochexian.top

[Q89] 判断表是否存在
来源：http://keb.daxiang520.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ofq.ehwqpu.com

[Q90] 生成序号列
来源：http://rir.yfazqb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nif.guannengcc.top

================================================================================
来源：http://fdu.cucudq.cn

R. Bash 专题
来源：http://uug.zhongyouzk.top

================================================================================
来源：http://mzf.fktsv.cn

[R01] shebang 与严格模式
来源：http://sje.0kj1m.cn

#!/usr/bin/env bash
来源：http://ogk.redwolf501.top

set -euo pipefail
来源：http://fzk.fengsongda.top

[R02] 变量赋值与使用
来源：http://qwk.yfazqb.com

name="Tom"; echo "$name"
来源：http://xjb.gaohongyu789.top

[R03] 只读变量
来源：http://gki.0kj1m.cn

readonly PI=3.14
来源：http://pce.ywan-chungtsiang.top

[R04] 位置参数
来源：http://umy.zhixingplan.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mxu.c1oappe.top

[R05] 参数默认值
来源：http://znd.fanxiaobao.xyz

name="${1:-default}"
来源：http://kng.yvedp.cn

[R06] 判断命令是否存在
来源：http://kia.fehbvm.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pqc.dianchejie.cn

[R07] if 判断文件
来源：http://qmo.yj20258888.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cgx.hongshengwenyu.top

[R08] 数值比较
来源：http://ijf.nanxuanxn.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ite.cdnleiting.top

[R09] 字符串比较
来源：http://vuz.quarkkingdee.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ebe.0kj1m.cn

[R10] 正则匹配
来源：http://upt.bbcook.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lnj.ctjpmb.com

[R11] case 多分支
来源：http://mki.havefunace.top

case "$1" in
来源：http://oig.wangdashe.top

start) echo "启动" ;;
来源：http://mty.zycfv.cn

stop)  echo "停止" ;;
来源：http://dfq.shanyushiyangtech.top

*)     echo "未知命令" ;;
来源：http://pnd.chenzaomai.com

esac
来源：http://wbq.uphjek.com

[R12] for 遍历文件
来源：http://zjt.xinyue.icu

for f in *.txt; do echo "$f"; done
来源：http://zpj.pycfn.com

[R13] for 计数循环
来源：http://dqp.cashguo.top

for i in {1..10}; do echo "$i"; done
来源：http://mql.nwbrower.top

[R14] C 风格 for
来源：http://geo.daxiang520.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gbk.kuanghao11.cn

[R15] while 逐行读文件
来源：http://tfi.yuanzhike.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gdw.chenlongwang.top

[R16] until 等待条件
来源：http://upg.yj20258.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hfj.guowangkeji.top

[R17] 数组定义与取值
来源：http://qfo.ydzc1.top

arr=(a b c); echo "${arr[0]}"
来源：http://zxb.epnwcf.com

[R18] 遍历数组
来源：http://xeh.shangyingyoupin.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vgn.shzxlz.cn

[R19] 数组长度
来源：http://kms.hongshengwenyu.top

echo "${#arr[@]}"
来源：http://hvk.cdnleiting.top

[R20] 关联数组（字典）
来源：http://mtk.zhixingplan.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bqd.0kj1m.cn

[R21] 字符串长度
来源：http://csq.tian-w.cn

echo "${#s}"
来源：http://qul.jinyuanbaomall.cn

[R22] 截取子串
来源：http://sxa.kuanghao11.cn

echo "${s:0:5}"
来源：http://owv.vehdjk.com

[R23] 字符串替换
来源：http://lyk.redwolf501.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pjn.svipenyu.cn

[R24] 大小写转换
来源：http://phe.xziqi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sbw.vehdjk.com

[R25] 去后缀 / 去前缀
来源：http://ais.gotoacloud.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lkp.ppjwa.cn

[R26] 命令替换
来源：http://pgc.shanyushiyangkeji.top

now=$(date +%F); echo "$now"
来源：http://peg.feifeiyinyue.top

[R27] 算术展开
来源：http://jjd.snrcjt.cn

echo $((1 + 2 * 3))
来源：http://llu.pengpengdd.cyou

[R28] 浮点运算
来源：http://hsk.9152youxi.cn

echo "scale=2; 10/3" | bc
来源：http://ktu.tianlin.xyz

[R29] 定义函数
来源：http://pwt.daxiang520.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rit.zhengqikj.top

[R30] 函数返回状态码
来源：http://qyq.dianchejie.cn

f() { return 0; }; f || echo "失败了"
来源：http://wwh.wangdashe.top

[R31] 局部变量
来源：http://wfv.shanyushiyangkeji.top

f() { local x=1; echo "$x"; }
来源：http://ubl.yuanzhike.top

[R32] 参数个数校验
来源：http://ozg.chenlongwang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rmp.ywan-chungtsiang.top

[R33] 捕获错误并提示行号
来源：http://hwb.yanxiufei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wqg.epnwcf.com

[R34] 退出时清理
来源：http://fkb.ppjwa.cn

trap 'rm -f "$tmp"' EXIT
来源：http://iry.cheryme.top

[R35] 后台执行并等待
来源：http://bca.quarkkingdee.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ney.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://qjj.hesvh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baw.vqdsnc.cn

[R37] 把输出赋给变量
来源：http://sxd.chenlongwang.top

files=$(ls -1)
来源：http://xcj.haohaochexian.top

[R38] 管道串联
来源：http://bpb.yonumen.top

cat a.txt | grep -i error | wc -l
来源：http://mri.chenlongwang.top

[R39] 重定向标准输出与错误
来源：http://etc.guowangkeji.top

cmd > out.log 2>&1
来源：http://ccb.wangshuangyany.cn

[R40] 追加写日志
来源：http://qdi.shangyingyoupin.top

echo "log" >> out.log
来源：http://lwr.xinyue.icu

[R41] 丢弃输出
来源：http://dqs.jianghu66.top

cmd >/dev/null 2>&1
来源：http://vlb.meibo888.top

[R42] 输入重定向
来源：http://kkm.zhoulong.xyz

wc -l < a.txt
来源：http://zjr.dashuyun.cn

[R43] 按名字查找文件
来源：http://ufg.xylfe.cn

find . -name "*.log" -type f
来源：http://uhg.shzxlz.cn

[R44] 按修改时间查找
来源：http://vtz.redwolf501.top

find . -mtime -7 -type f
来源：http://dxe.dianchejie.cn

[R45] 批量删除
来源：http://ats.jlsjyb.cn

find . -name "*.tmp" -delete
来源：http://cia.fengsongda.top

[R46] 递归替换文件内容
来源：http://nqv.haohaochexian.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nab.0kj1m.cn

[R47] sed 单行替换
来源：http://vlf.fzhhl.top

sed -i 's/foo/bar/g' a.txt
来源：http://yqr.guannengcc.top

[R48] awk 取指定列
来源：http://mvt.9152youxi.cn

awk '{print $1, $3}' a.txt
来源：http://vlh.zycfv.cn

[R49] awk 带条件
来源：http://hnd.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://khx.cheryme.top

[R50] awk 求和
来源：http://stq.hywenlv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pyb.meibo888.top

[R51] 排序去重取前几
来源：http://zpb.yj20258.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pdr.quarkkingdee.top

[R52] 统计行数
来源：http://ulg.zhengqikj.top

wc -l a.txt
来源：http://nbz.bjfxy.top

[R53] 查看文件头与实时尾
来源：http://tfu.yj20258888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xch.jinqigfzy.top

[R54] 比较两个文件
来源：http://pft.vqdsnc.cn

diff a.txt b.txt
来源：http://hwx.xingfuxueyuan.xyz

[R55] 压缩与解压
来源：http://ayw.tanke756.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dji.jinqigfzy.top

[R56] 远程拷贝
来源：http://xxx.chenjidiqi.icu

scp file user@host:/path/
来源：http://bss.bjfxy.top

[R57] 远程执行命令
来源：http://bkh.52xcode.cn

ssh user@host 'uptime'
来源：http://fcx.jinghuilouyu.cn

[R58] 下载文件
来源：http://xuv.redwolf501.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hco.xziqi.cn

[R59] 发 POST JSON
来源：http://mws.svipenyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bma.jqgfzy.top

[R60] 只看 HTTP 状态码
来源：http://dei.sweek.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zpa.chenjidiqi.icu

[R61] 磁盘占用
来源：http://cmc.shanyushiyangtech.top

df -h;  du -sh *
来源：http://kxe.tarul.cn

[R62] 找最占空间的文件
来源：http://ird.jinqigfzy.top

du -ah . | sort -rh | head -10
来源：http://iid.fanxiaobao.xyz

[R63] 内存与进程
来源：http://mgc.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://pjl.ivvv.top

[R64] 结束进程
来源：http://fwg.cheryme.top

kill -9 $(pgrep -f app.py)
来源：http://ydv.nanxuanxn.top

[R65] 查看端口占用
来源：http://avr.316326.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://szc.pycfn.com

[R66] 定时任务
来源：http://mkj.jqgufenzy.top

crontab -e;  crontab -l
来源：http://ldt.yuanzhike.top

[R67] 生成随机十六进制串
来源：http://gpl.ydzc1.top


<!-- 参考信息 -->