代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://frm.zhijiandao.cn

[Q24] 去重
来源：http://hhi.birdmap.top

SELECT DISTINCT city FROM users;
来源：http://lqr.hnqzz.top

[Q25] 只取前 N 条
来源：http://xpo.9152youxi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://emi.yonumen.top

[Q26] 计数
来源：http://lxz.jinqigfzy.top

SELECT COUNT(*) FROM users;
来源：http://ebc.ctjpmb.com

[Q27] 条件计数
来源：http://krt.zhijiandao.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aui.dashuyun.cn

[Q28] 求和与平均
来源：http://win.vehdjk.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://niq.zycfv.cn

[Q29] 最大最小值
来源：http://wpp.guowangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qsn.0kj1m.cn

[Q30] 分组统计
来源：http://lwr.hammf.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qvt.kuanghao11.cn

[Q31] 分组后过滤
来源：http://rho.yvedp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ozo.fktsv.cn

[Q32] 分组拼接字符串
来源：http://aca.xziqi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lzp.shuidangran.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nxm.feifeiyinyue.top

[Q33] 多列分组
来源：http://hzw.cucudq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fqi.fehbvm.com

[Q34] 每组取第一条
来源：http://rig.gzhubu.top

SELECT * FROM (
来源：http://csr.gogol.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jej.zhoulong.xyz

) t WHERE rn = 1;
来源：http://wbj.xingfuxueyuan.xyz

[Q35] 内连接
来源：http://bzg.iojbl.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://suo.svipenyu.cn

[Q36] 左连接
来源：http://mlv.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yzv.cdnleiting.top

[Q37] 右连接
来源：http://vxk.chenzaomai.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xlx.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yax.gzhubu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xik.haohaochexian.top

[Q39] 自连接（查上下级）
来源：http://fua.sxryk.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cmf.316326.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://omz.zhengqikj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wtl.hfpthk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sej.yuxming.cn

[Q41] 多表连接
来源：http://nby.fktsv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tml.bjfxy.top

JOIN users u ON u.id = o.user_id
来源：http://mdw.hnxiangtu.top

JOIN products p ON p.id = o.product_id;
来源：http://cas.zhoulong.xyz

[Q42] 连接条件附加过滤
来源：http://nxp.xylfe.cn

SELECT u.name, o.amount FROM users u
来源：http://ndf.nanxuanxn.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wwv.havefunace.top

[Q43] 标量子查询
来源：http://dln.yueranfly.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xvf.yangfankeji.com

[Q44] IN 子查询
来源：http://blt.sufxvd.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ybr.zhiwuduotai.top

[Q45] EXISTS 判断存在
来源：http://xss.daxiang520.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iue.ydjk.org.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wll.haohaochexian.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fsi.ivvv.top

[Q47] 与平均值比较
来源：http://jrf.fehbvm.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wuy.jqgfzy.top

[Q48] CTE 公用表表达式
来源：http://xnk.zhaomingkeji.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pvs.fanxiaobao.xyz

SELECT * FROM t WHERE c > 5;
来源：http://mty.yvedp.cn

[Q49] 更新单行
来源：http://ftl.yj20258.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uzp.tarul.cn

[Q50] 批量更新
来源：http://gfc.fehbvm.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://itf.gotoacloud.top

[Q51] 用子查询更新
来源：http://vsl.yonumen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fnc.redwolf501.top

[Q52] 删除指定行
来源：http://sqr.redwolf501.top

DELETE FROM users WHERE id = 10;
来源：http://mjl.zhoulong.xyz

[Q53] 按条件删除
来源：http://cyt.cashguo.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vam.dianchejie.cn

[Q54] 清空表
来源：http://fbl.cashguo.top

TRUNCATE TABLE logs;
来源：http://igy.yanxiufei.cn

[Q55] 排名（并列占位）
来源：http://uxd.hesvh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lou.fehbvm.com

[Q56] 密集排名（并列不占位）
来源：http://mel.xingfuxueyuan.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ehu.sweek.top

[Q57] 行号
来源：http://muy.xziqi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ttb.sufxvd.cn

[Q58] 累计求和
来源：http://uix.zdqjudy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uiq.iojbl.cn

[Q59] 分组内累计
来源：http://wle.birdmap.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nfo.guowangkeji.top

[Q60] 取上一行 / 下一行
来源：http://dmp.havefunace.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bqa.zhixingplan.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pyl.guowangkeji.top

[Q61] 移动平均
来源：http://ysu.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lvw.yangfankeji.com

[Q62] 分组占比
来源：http://xji.sxryk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cll.daria6918.cn

[Q63] 开启事务
来源：http://yoy.fanxiaobao.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://env.sjlbkw.cn

[Q64] 提交事务
来源：http://nfw.c1oappe.top

COMMIT;
来源：http://ban.shanyushiyangkeji.top

[Q65] 回滚事务
来源：http://wbi.yueranfly.top

ROLLBACK;
来源：http://sxk.9152youxi.cn

[Q66] 行锁查询
来源：http://qqc.zhiwuduotai.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://emk.52xcode.cn

[Q67] 设置隔离级别
来源：http://fof.zhoulong.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lig.ctjpmb.com

[Q68] 保存点
来源：http://tuh.vqdsnc.cn

SAVEPOINT sp1;
来源：http://bzs.zhijiandao.cn

ROLLBACK TO sp1;
来源：http://kvm.birdmap.top

[Q69] 查看执行计划
来源：http://aug.snrcjt.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wtm.yanxiufei.cn

[Q70] 更新统计信息
来源：http://gry.yonumen.top

ANALYZE TABLE users;
来源：http://asw.smart0.xyz

[Q71] 查看建表语句
来源：http://vjd.zycfv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cbr.guowangkeji.top

[Q72] 查看索引
来源：http://pju.hfpthk.cn

SHOW INDEX FROM users;
来源：http://whj.ppjwa.cn

[Q73] 查看表状态
来源：http://fiw.fengsongda.top

SHOW TABLE STATUS LIKE 'users';
来源：http://yak.andypj.xyz

[Q74] 强制使用索引
来源：http://vyy.iojbl.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gun.xziqi.cn

[Q75] 日期格式化
来源：http://xnn.yuanzhike.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rtn.hfpthk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pqy.daxiang520.top

[Q76] 按天统计
来源：http://djv.hammf.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zyz.jiagoushi.top

[Q77] 时间加减
来源：http://zdi.ydzc1.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://azo.andypj.xyz

[Q78] 当前时间
来源：http://scp.tian-w.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xsx.fengsongda.top

[Q79] 字符串拼接
来源：http://klk.tianlin.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hwi.9152youxi.cn

[Q80] 字符串截取
来源：http://ipr.0kj1m.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dok.redwolf501.top

[Q81] 字符串替换
来源：http://drw.zdqjudy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kqv.snrcjt.cn

[Q82] 字符长度与字节长度
来源：http://mdv.gaohongyu789.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jya.shanyushiyangtech.top

[Q83] 大小写转换
来源：http://wts.feifeiyinyue.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://puv.birdmap.top

[Q84] 去除首尾空格
来源：http://uwg.aibaodan.cn

SELECT TRIM(name) FROM users;
来源：http://jog.jyoumei.cn

[Q85] 数值取整
来源：http://sim.hysaishi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ubi.jinghuilouyu.cn

[Q86] 读取 JSON 字段
来源：http://dzr.kuanghao11.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zbg.xylfe.cn

[Q87] JSON 字段做条件
来源：http://xni.cdnleiting.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nrz.xylfe.cn

[Q88] 行转列（条件聚合）
来源：http://goa.chenjidiqi.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iuy.c1oappe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mvd.andypj.xyz

[Q89] 判断表是否存在
来源：http://tqv.daria6918.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ggi.fanxiaobao.xyz

[Q90] 生成序号列
来源：http://nfa.jyoumei.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vfz.cheryme.top

================================================================================
来源：http://dvj.gzhubu.top

R. Bash 专题
来源：http://akk.tarul.cn

================================================================================
来源：http://aek.xingfuxueyuan.xyz

[R01] shebang 与严格模式
来源：http://vnq.shangyingyoupin.top

#!/usr/bin/env bash
来源：http://yjk.chenzaomai.com

set -euo pipefail
来源：http://dgk.haohaochexian.top

[R02] 变量赋值与使用
来源：http://asl.zdqjudy.top

name="Tom"; echo "$name"
来源：http://oxy.dashuyun.cn

[R03] 只读变量
来源：http://htn.hysaishi.cn

readonly PI=3.14
来源：http://zjv.ydjk.org.cn

[R04] 位置参数
来源：http://qgs.hysaishi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sdy.sjlbkw.cn

[R05] 参数默认值
来源：http://can.cdnleiting.top

name="${1:-default}"
来源：http://gyk.chenzaomai.com

[R06] 判断命令是否存在
来源：http://qpn.cdnleiting.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tnn.nwbrower.top

[R07] if 判断文件
来源：http://lzi.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wrr.ctjpmb.com

[R08] 数值比较
来源：http://eng.sufxvd.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pxd.dashuyun.cn

[R09] 字符串比较
来源：http://vew.dianchejie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fih.fengsongda.top

[R10] 正则匹配
来源：http://ltn.shzxlz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hgx.vehdjk.com

[R11] case 多分支
来源：http://ifk.dashuyun.cn

case "$1" in
来源：http://tge.fengsongda.top

start) echo "启动" ;;
来源：http://wby.yuanzhike.top

stop)  echo "停止" ;;
来源：http://mcz.quarkkingdee.top

*)     echo "未知命令" ;;
来源：http://mtl.cheryme.top

esac
来源：http://rhb.hcnkem.com

[R12] for 遍历文件
来源：http://ism.wangshuangyany.cn

for f in *.txt; do echo "$f"; done
来源：http://sqx.guannengcc.top

[R13] for 计数循环
来源：http://olh.xylfe.cn

for i in {1..10}; do echo "$i"; done
来源：http://lvs.zhongyouzk.top

[R14] C 风格 for
来源：http://lia.meibo888.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xpi.fzhhl.top

[R15] while 逐行读文件
来源：http://krc.aibaodan.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pnf.cucudq.cn

[R16] until 等待条件
来源：http://bmv.52xcode.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gxd.zycfv.cn

[R17] 数组定义与取值
来源：http://vbf.fzhhl.top

arr=(a b c); echo "${arr[0]}"
来源：http://fbp.gogol.net.cn

[R18] 遍历数组
来源：http://vwb.zhoulong.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hog.bjfxy.top

[R19] 数组长度
来源：http://kxf.svipenyu.cn

echo "${#arr[@]}"
来源：http://vam.kuanghao11.cn

[R20] 关联数组（字典）
来源：http://ueu.316326.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jcm.shangyingyoupin.top

[R21] 字符串长度
来源：http://aur.xziqi.cn

echo "${#s}"
来源：http://iox.316326.xyz

[R22] 截取子串
来源：http://ltx.vqdsnc.cn

echo "${s:0:5}"
来源：http://tcv.jinyuanbaomall.cn

[R23] 字符串替换
来源：http://iiw.sxryk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hfl.guannengcc.top

[R24] 大小写转换
来源：http://nar.nanxinkj.top

echo "${s^^}"; echo "${s,,}"
来源：http://xuo.fzhhl.top

[R25] 去后缀 / 去前缀
来源：http://vie.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vhl.sxryk.cn

[R26] 命令替换
来源：http://rbm.yuanzhike.top

now=$(date +%F); echo "$now"
来源：http://dwu.yuanzhike.top

[R27] 算术展开
来源：http://clu.bjfxy.top

echo $((1 + 2 * 3))
来源：http://rdc.xuanzx.com

[R28] 浮点运算
来源：http://rst.tian-w.cn

echo "scale=2; 10/3" | bc
来源：http://waq.ppjwa.cn

[R29] 定义函数
来源：http://lso.xuetiantiany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://grh.tianlin.xyz

[R30] 函数返回状态码
来源：http://rep.meibo888.top

f() { return 0; }; f || echo "失败了"
来源：http://dfz.316326.xyz

[R31] 局部变量
来源：http://dox.jqgfzy.top

f() { local x=1; echo "$x"; }
来源：http://btq.52xcode.cn

[R32] 参数个数校验
来源：http://xoe.uphjek.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://huo.nanxuanxn.top

[R33] 捕获错误并提示行号
来源：http://ymd.zhixingplan.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uhv.yangfankeji.com

[R34] 退出时清理
来源：http://lvr.ydzc1.top

trap 'rm -f "$tmp"' EXIT
来源：http://zjf.zhengqikj.top

[R35] 后台执行并等待
来源：http://dyp.cheryme.top

sleep 5 & pid=$!; wait "$pid"
来源：http://nax.jqgfzy.top

[R36] 并发执行多个任务
来源：http://jbz.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mvb.jinghuilouyu.cn

[R37] 把输出赋给变量
来源：http://slo.9152youxi.cn

files=$(ls -1)
来源：http://iru.52xcode.cn

[R38] 管道串联
来源：http://qql.jqgufenzy.top

cat a.txt | grep -i error | wc -l
来源：http://hws.316326.xyz

[R39] 重定向标准输出与错误
来源：http://cll.yj202588.top

cmd > out.log 2>&1
来源：http://xex.ydzc1.top

[R40] 追加写日志
来源：http://jhl.guannengcc.top

echo "log" >> out.log
来源：http://kfy.guannengcc.top

[R41] 丢弃输出
来源：http://bhd.jianghu66.top

cmd >/dev/null 2>&1
来源：http://pif.aibaodan.cn

[R42] 输入重定向
来源：http://jak.hcnkem.com

wc -l < a.txt
来源：http://grx.jqgfzy.top

[R43] 按名字查找文件
来源：http://egw.hongshengwenyu.top

find . -name "*.log" -type f
来源：http://ofh.yuanzhike.top

[R44] 按修改时间查找
来源：http://dzk.zhiwuduotai.top

find . -mtime -7 -type f
来源：http://hfg.andypj.xyz

[R45] 批量删除
来源：http://pan.yj20258.top

find . -name "*.tmp" -delete
来源：http://eek.jianghu66.top

[R46] 递归替换文件内容
来源：http://vrm.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ybx.gogol.net.cn

[R47] sed 单行替换
来源：http://gia.zdqjudy.top

sed -i 's/foo/bar/g' a.txt
来源：http://itc.yuxming.cn

[R48] awk 取指定列
来源：http://feb.fzhhl.top

awk '{print $1, $3}' a.txt
来源：http://erd.chenzaomai.com

[R49] awk 带条件
来源：http://nhc.chenzaomai.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://txq.sxryk.cn

[R50] awk 求和
来源：http://ysd.jqgfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://vdr.jiagoushi.top

[R51] 排序去重取前几
来源：http://sov.aizwys.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rjl.nwbrower.top

[R52] 统计行数
来源：http://gew.fzhhl.top

wc -l a.txt
来源：http://ovo.feifeiyinyue.top

[R53] 查看文件头与实时尾
来源：http://yap.ctjpmb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vyr.meibo888.top

[R54] 比较两个文件
来源：http://zem.jinghuilouyu.cn

diff a.txt b.txt
来源：http://yls.xuetiantiany.cn

[R55] 压缩与解压
来源：http://dqx.tarul.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jrk.tian-w.cn

[R56] 远程拷贝
来源：http://mxk.zdqjudy.top

scp file user@host:/path/
来源：http://ydk.cdnleiting.top

[R57] 远程执行命令
来源：http://ezx.xylfe.cn

ssh user@host 'uptime'
来源：http://qdl.hammf.cn

[R58] 下载文件
来源：http://jdn.hnxiangtu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://biz.ydzc1.top

[R59] 发 POST JSON
来源：http://vuc.hesvh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zdi.yueranfly.top

[R60] 只看 HTTP 状态码
来源：http://ryj.gogol.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://znu.tarul.cn

[R61] 磁盘占用
来源：http://wdj.sufxvd.cn

df -h;  du -sh *
来源：http://sjr.jinyuanbaomall.cn

[R62] 找最占空间的文件
来源：http://slq.cucudq.cn

du -ah . | sort -rh | head -10
来源：http://uva.xziqi.cn

[R63] 内存与进程
来源：http://nqo.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://oup.snrcjt.cn

[R64] 结束进程
来源：http://zpy.fzhhl.top

kill -9 $(pgrep -f app.py)
来源：http://tzn.jlsjyb.cn

[R65] 查看端口占用
来源：http://iky.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bte.sufxvd.cn

[R66] 定时任务
来源：http://hmi.ywan-chungtsiang.top

crontab -e;  crontab -l
来源：http://tly.zhengqikj.top

[R67] 生成随机十六进制串
来源：http://itl.smart0.xyz

openssl rand -hex 16
来源：http://vqz.haohaochexian.top

[R68] 计算文件校验值
来源：http://mln.shanyushiyangtech.top

sha256sum a.txt;  md5sum a.txt
来源：http://rxz.tarul.cn

[R69] 生成随机密码
来源：http://tfc.sjlbkw.cn

head -c 16 /dev/urandom | base64
来源：http://gpl.ydjk.org.cn

[R70] 时间戳与互转
来源：http://sra.smart0.xyz

date +%s;  date -d @1700000000
来源：http://qow.jiagoushi.top

[R71] 日期格式化
来源：http://gpe.havefunace.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ley.zhaomingkeji.xyz

[R72] 等待端口就绪
来源：http://bng.epnwcf.com

until nc -z localhost 3306; do sleep 1; done
来源：http://puf.havefunace.top

[R73] 分割大日志
来源：http://oxp.yuanzhike.top


<!-- 参考信息 -->