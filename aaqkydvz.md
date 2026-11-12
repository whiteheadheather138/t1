代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rov.guannengcc.top

[Q20] IN 列表
来源：http://hkl.316326.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://apm.zdqjudy.top

[Q21] 空值判断
来源：http://jpp.ehwqpu.com

SELECT * FROM users WHERE email IS NULL;
来源：http://nde.havefunace.top

[Q22] 排序
来源：http://gly.daxiang520.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ond.guowangkeji.top

[Q23] 分页
来源：http://egs.nanxinkj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hsa.sjlbkw.cn

[Q24] 去重
来源：http://zbd.uphjek.com

SELECT DISTINCT city FROM users;
来源：http://hho.sufxvd.cn

[Q25] 只取前 N 条
来源：http://bls.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://twz.xziqi.cn

[Q26] 计数
来源：http://xms.jqgfzy.top

SELECT COUNT(*) FROM users;
来源：http://paq.nwbrower.top

[Q27] 条件计数
来源：http://kir.daria6918.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ntk.xuetiantiany.cn

[Q28] 求和与平均
来源：http://ekd.iojbl.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cbl.hnqzz.top

[Q29] 最大最小值
来源：http://xrg.zdqjudy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://svq.jyoumei.cn

[Q30] 分组统计
来源：http://eua.bbcook.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://flk.tian-w.cn

[Q31] 分组后过滤
来源：http://pxp.sufxvd.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cfo.fzhhl.top

[Q32] 分组拼接字符串
来源：http://nqm.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bvq.zhaomingkeji.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://afe.ybcxt.top

[Q33] 多列分组
来源：http://ece.chenzaomai.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yps.hywenlv.cn

[Q34] 每组取第一条
来源：http://bat.yangfankeji.com

SELECT * FROM (
来源：http://prp.hnqzz.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fhn.snrcjt.cn

) t WHERE rn = 1;
来源：http://ikx.wangshuangyany.cn

[Q35] 内连接
来源：http://rjx.jinqigfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aqk.fktsv.cn

[Q36] 左连接
来源：http://ceu.hfpthk.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://omg.yonumen.top

[Q37] 右连接
来源：http://hcp.cqqwz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yzx.gogol.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hck.ydjk.org.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tiy.ehwqpu.com

[Q39] 自连接（查上下级）
来源：http://kjf.yuxming.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kps.nanxinkj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jby.shzxlz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yzz.havefunace.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gpo.chenzaomai.com

[Q41] 多表连接
来源：http://nmw.zycfv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://twk.daxiang520.top

JOIN users u ON u.id = o.user_id
来源：http://vgc.feifeiyinyue.top

JOIN products p ON p.id = o.product_id;
来源：http://vlw.shangyingyoupin.top

[Q42] 连接条件附加过滤
来源：http://vlo.yuanzhike.top

SELECT u.name, o.amount FROM users u
来源：http://nei.gaohongyu789.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bew.cheryme.top

[Q43] 标量子查询
来源：http://khr.zhongyouzk.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mvn.yfazqb.com

[Q44] IN 子查询
来源：http://vgt.hcnkem.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://afk.xylfe.cn

[Q45] EXISTS 判断存在
来源：http://nwj.hfpthk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://smp.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cbe.sjlbkw.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qrd.kuanghao11.cn

[Q47] 与平均值比较
来源：http://ajr.sxryk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://miu.fktsv.cn

[Q48] CTE 公用表表达式
来源：http://zep.guannengcc.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zsf.fehbvm.com

SELECT * FROM t WHERE c > 5;
来源：http://hzb.bbcook.cn

[Q49] 更新单行
来源：http://bgc.uphjek.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bey.zdbjq.cn

[Q50] 批量更新
来源：http://nyg.xylfe.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bqa.zdbjq.cn

[Q51] 用子查询更新
来源：http://udy.havefunace.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kah.yvedp.cn

[Q52] 删除指定行
来源：http://xms.jinqigfzy.top

DELETE FROM users WHERE id = 10;
来源：http://gwp.cdnleiting.top

[Q53] 按条件删除
来源：http://ilv.sufxvd.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mki.zhijiandao.cn

[Q54] 清空表
来源：http://alr.gotoacloud.top

TRUNCATE TABLE logs;
来源：http://hzq.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://dns.cucudq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://emd.hnxiangtu.top

[Q56] 密集排名（并列不占位）
来源：http://pig.kuanghao11.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sjy.gaohongyu789.top

[Q57] 行号
来源：http://dsz.wangshuangyany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ffz.chenzaomai.com

[Q58] 累计求和
来源：http://voi.yj20258.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://erz.wangshuangyany.cn

[Q59] 分组内累计
来源：http://soh.shzxlz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jnj.bjfxy.top

[Q60] 取上一行 / 下一行
来源：http://mhk.iojbl.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pvq.chenlongwang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vwa.shanyushiyangtech.top

[Q61] 移动平均
来源：http://xeg.hcnkem.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://itn.ybcxt.top

[Q62] 分组占比
来源：http://adc.xinyue.icu

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pqx.jinqigufen.top

[Q63] 开启事务
来源：http://sta.jinqigfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ils.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://fqh.dashuyun.cn

COMMIT;
来源：http://jjl.guannengcc.top

[Q65] 回滚事务
来源：http://qfq.dashuyun.cn

ROLLBACK;
来源：http://ezt.svipenyu.cn

[Q66] 行锁查询
来源：http://avy.hfpthk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pti.ppjwa.cn

[Q67] 设置隔离级别
来源：http://pim.aibaodan.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://coh.zycfv.cn

[Q68] 保存点
来源：http://cqp.zhongyouzk.top

SAVEPOINT sp1;
来源：http://lok.xziqi.cn

ROLLBACK TO sp1;
来源：http://rjo.sufxvd.cn

[Q69] 查看执行计划
来源：http://bnm.zycfv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wma.jinqigfzy.top

[Q70] 更新统计信息
来源：http://pyp.fengsongda.top

ANALYZE TABLE users;
来源：http://wax.ydzc1.top

[Q71] 查看建表语句
来源：http://dre.andypj.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gdd.fanxiaobao.xyz

[Q72] 查看索引
来源：http://uej.jiagoushi.top

SHOW INDEX FROM users;
来源：http://fry.xuanzx.com

[Q73] 查看表状态
来源：http://sur.yonumen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xug.52xcode.cn

[Q74] 强制使用索引
来源：http://frp.hesvh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blr.jyoumei.cn

[Q75] 日期格式化
来源：http://yxd.cheryme.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pwc.aibaodan.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kzf.cqqwz.cn

[Q76] 按天统计
来源：http://sza.ppjwa.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wnf.shuidangran.top

[Q77] 时间加减
来源：http://zah.fktsv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://roq.tanke756.top

[Q78] 当前时间
来源：http://got.gaohongyu789.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ubi.fktsv.cn

[Q79] 字符串拼接
来源：http://mrp.hammf.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nav.kuanghao11.cn

[Q80] 字符串截取
来源：http://yte.tian-w.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sqn.tianlin.xyz

[Q81] 字符串替换
来源：http://mkh.ctjpmb.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://weu.tianlin.xyz

[Q82] 字符长度与字节长度
来源：http://uvc.jinghuilouyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hxs.ydzc1.top

[Q83] 大小写转换
来源：http://mgs.xinyue.icu

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bsn.fengsongda.top

[Q84] 去除首尾空格
来源：http://vye.sysykeji.top

SELECT TRIM(name) FROM users;
来源：http://vuo.smart0.xyz

[Q85] 数值取整
来源：http://dqf.zhongyouzk.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uac.52xcode.cn

[Q86] 读取 JSON 字段
来源：http://clp.daria6918.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://izw.jinqigfzy.top

[Q87] JSON 字段做条件
来源：http://fxb.meibo888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qqs.nanxinkj.top

[Q88] 行转列（条件聚合）
来源：http://cym.hnxiangtu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ehk.fanxiaobao.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vlu.ehwqpu.com

[Q89] 判断表是否存在
来源：http://jdg.nwbrower.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wcg.cqqwz.cn

[Q90] 生成序号列
来源：http://vfz.zhoulong.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ltb.meibo888.top

================================================================================
来源：http://mya.bbcook.cn

R. Bash 专题
来源：http://mvt.shzxlz.cn

================================================================================
来源：http://upi.yvedp.cn

[R01] shebang 与严格模式
来源：http://qnr.yueranfly.top

#!/usr/bin/env bash
来源：http://hju.yuxming.cn

set -euo pipefail
来源：http://zrd.yuxming.cn

[R02] 变量赋值与使用
来源：http://erl.guannengcc.top

name="Tom"; echo "$name"
来源：http://hsx.ybcxt.top

[R03] 只读变量
来源：http://qzw.jinqigufen.top

readonly PI=3.14
来源：http://qyy.zhengqikj.top

[R04] 位置参数
来源：http://ymz.iojbl.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vcg.ivvv.top

[R05] 参数默认值
来源：http://kpb.ywan-chungtsiang.top

name="${1:-default}"
来源：http://uvc.ybcxt.top

[R06] 判断命令是否存在
来源：http://ffa.pycfn.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sxz.cheryme.top

[R07] if 判断文件
来源：http://eeb.zhoulong.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ncz.cucudq.cn

[R08] 数值比较
来源：http://ugn.jlsjyb.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rld.chenzaomai.com

[R09] 字符串比较
来源：http://zzz.fengsongda.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cky.gaohongyu789.top

[R10] 正则匹配
来源：http://pwa.sjlbkw.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uni.xuanzx.com

[R11] case 多分支
来源：http://unc.xziqi.cn

case "$1" in
来源：http://uou.ivvv.top

start) echo "启动" ;;
来源：http://lzn.zdbjq.cn

stop)  echo "停止" ;;
来源：http://lvc.52xcode.cn

*)     echo "未知命令" ;;
来源：http://zut.gaohongyu789.top

esac
来源：http://vrs.cashguo.top

[R12] for 遍历文件
来源：http://lba.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://ckb.zycfv.cn

[R13] for 计数循环
来源：http://tpl.jqgfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://eqh.redwolf501.top

[R14] C 风格 for
来源：http://poe.yuxming.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://llm.chenzaomai.com

[R15] while 逐行读文件
来源：http://rup.hfpthk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lim.zhoulong.xyz

[R16] until 等待条件
来源：http://aca.cucudq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gdx.hysaishi.cn

[R17] 数组定义与取值
来源：http://fdc.yangfankeji.com

arr=(a b c); echo "${arr[0]}"
来源：http://zfg.yueranfly.top

[R18] 遍历数组
来源：http://mqy.hnqzz.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ued.fengsongda.top

[R19] 数组长度
来源：http://vyh.jinqigufen.top

echo "${#arr[@]}"
来源：http://fqa.cdnleiting.top

[R20] 关联数组（字典）
来源：http://lrs.zdqjudy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xul.cdnleiting.top

[R21] 字符串长度
来源：http://dmd.feifeiyinyue.top

echo "${#s}"
来源：http://bzc.aibaodan.cn

[R22] 截取子串
来源：http://lua.fengsongda.top

echo "${s:0:5}"
来源：http://sqr.yj202588.top

[R23] 字符串替换
来源：http://rwn.gogol.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://odr.cheryme.top

[R24] 大小写转换
来源：http://wqo.sweek.top

echo "${s^^}"; echo "${s,,}"
来源：http://kem.sxryk.cn

[R25] 去后缀 / 去前缀
来源：http://plr.xuanzx.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://pan.jiagoushi.top

[R26] 命令替换
来源：http://hof.daria6918.cn

now=$(date +%F); echo "$now"
来源：http://qvk.iojbl.cn

[R27] 算术展开
来源：http://usk.zycfv.cn

echo $((1 + 2 * 3))
来源：http://coa.tianlin.xyz

[R28] 浮点运算
来源：http://wpp.jyoumei.cn

echo "scale=2; 10/3" | bc
来源：http://tpo.guannengcc.top

[R29] 定义函数
来源：http://nsf.aizwys.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kyj.hnxiangtu.top

[R30] 函数返回状态码
来源：http://fig.xinyue.icu

f() { return 0; }; f || echo "失败了"
来源：http://jib.wangshuangyany.cn

[R31] 局部变量
来源：http://rxk.yuanzhike.top

f() { local x=1; echo "$x"; }
来源：http://ifm.yj20258.top

[R32] 参数个数校验
来源：http://ydv.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cov.smart0.xyz

[R33] 捕获错误并提示行号
来源：http://klh.zdqjudy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bgc.meibo888.top

[R34] 退出时清理
来源：http://iws.hammf.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lhi.nwbrower.top

[R35] 后台执行并等待
来源：http://rij.cdnleiting.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jid.yj202588.top

[R36] 并发执行多个任务
来源：http://wll.zycfv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lgx.guowangkeji.top

[R37] 把输出赋给变量
来源：http://ftn.yvedp.cn

files=$(ls -1)
来源：http://neh.svipenyu.cn

[R38] 管道串联
来源：http://llj.birdmap.top

cat a.txt | grep -i error | wc -l
来源：http://yhi.yangfankeji.com

[R39] 重定向标准输出与错误
来源：http://dyk.tianlin.xyz

cmd > out.log 2>&1
来源：http://mji.gogol.net.cn

[R40] 追加写日志
来源：http://fyt.iojbl.cn

echo "log" >> out.log
来源：http://pjy.feifeiyinyue.top

[R41] 丢弃输出
来源：http://zif.hcnkem.com

cmd >/dev/null 2>&1
来源：http://oun.yuxming.cn

[R42] 输入重定向
来源：http://poi.0kj1m.cn

wc -l < a.txt
来源：http://huq.fzhhl.top

[R43] 按名字查找文件
来源：http://pcj.smart0.xyz

find . -name "*.log" -type f
来源：http://mkg.yuanzhike.top

[R44] 按修改时间查找
来源：http://fjr.hfpthk.cn

find . -mtime -7 -type f
来源：http://ewj.hywenlv.cn

[R45] 批量删除
来源：http://bgt.ybcxt.top

find . -name "*.tmp" -delete
来源：http://mus.uphjek.com

[R46] 递归替换文件内容
来源：http://oeu.gzhubu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xkk.jianghu66.top

[R47] sed 单行替换
来源：http://hoo.jqgufenzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://nkf.hfpthk.cn

[R48] awk 取指定列
来源：http://qzz.0kj1m.cn

awk '{print $1, $3}' a.txt
来源：http://sfv.tian-w.cn

[R49] awk 带条件
来源：http://wdi.nwbrower.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lqo.zhoulong.xyz

[R50] awk 求和
来源：http://xgo.zycfv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://iwt.fehbvm.com

[R51] 排序去重取前几
来源：http://qfa.zhijiandao.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yur.fanxiaobao.xyz

[R52] 统计行数
来源：http://tvc.kuanghao11.cn

wc -l a.txt
来源：http://jul.smart0.xyz

[R53] 查看文件头与实时尾
来源：http://bzn.ctjpmb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fge.sufxvd.cn

[R54] 比较两个文件
来源：http://tub.xziqi.cn

diff a.txt b.txt
来源：http://tqa.feifeiyinyue.top

[R55] 压缩与解压
来源：http://xnt.nwbrower.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qgx.xuanzx.com

[R56] 远程拷贝
来源：http://ltj.shanyushiyangtech.top

scp file user@host:/path/
来源：http://vlp.shanyushiyangkeji.top

[R57] 远程执行命令
来源：http://qpy.jinghuilouyu.cn

ssh user@host 'uptime'
来源：http://taf.jianghu66.top

[R58] 下载文件
来源：http://svi.ivvv.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qrg.hysaishi.cn

[R59] 发 POST JSON
来源：http://lcq.hcnkem.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rew.jinqigufen.top

[R60] 只看 HTTP 状态码
来源：http://jxx.quarkkingdee.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mgo.shangyingyoupin.top

[R61] 磁盘占用
来源：http://akb.pengpengdd.cyou

df -h;  du -sh *
来源：http://uck.cucudq.cn

[R62] 找最占空间的文件
来源：http://hgr.ydjk.org.cn

du -ah . | sort -rh | head -10
来源：http://ozr.sxryk.cn

[R63] 内存与进程
来源：http://nzb.pengpengdd.cyou

free -h;  ps aux | grep nginx
来源：http://ufq.fengsongda.top

[R64] 结束进程
来源：http://plx.jqgfzy.top

kill -9 $(pgrep -f app.py)
来源：http://nbc.zhiwuduotai.top

[R65] 查看端口占用
来源：http://aql.cqqwz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qtm.aizwys.cn

[R66] 定时任务
来源：http://epk.shanyushiyangtech.top

crontab -e;  crontab -l
来源：http://urq.xuanzx.com

[R67] 生成随机十六进制串
来源：http://def.cheryme.top

openssl rand -hex 16
来源：http://sfw.hysaishi.cn

[R68] 计算文件校验值
来源：http://tno.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ihk.yj20258.top

[R69] 生成随机密码
来源：http://tpx.bbcook.cn


<!-- 参考信息 -->