代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://aoc.jinqigufen.top

[Q22] 排序
来源：http://pin.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://obv.sjlbkw.cn

[Q23] 分页
来源：http://rdu.nanxuanxn.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lni.ehwqpu.com

[Q24] 去重
来源：http://frh.feifeiyinyue.top

SELECT DISTINCT city FROM users;
来源：http://vml.dashuyun.cn

[Q25] 只取前 N 条
来源：http://rfs.xylfe.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dsg.tianlin.xyz

[Q26] 计数
来源：http://cst.smart0.xyz

SELECT COUNT(*) FROM users;
来源：http://tzn.uphjek.com

[Q27] 条件计数
来源：http://ktp.jyoumei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://seq.pengpengdd.cyou

[Q28] 求和与平均
来源：http://nyf.havefunace.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tzp.nanxuanxn.top

[Q29] 最大最小值
来源：http://uly.gaohongyu789.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mmx.hesvh.cn

[Q30] 分组统计
来源：http://jbx.0kj1m.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bft.cheryme.top

[Q31] 分组后过滤
来源：http://fll.yj202588.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ctg.yj20258.top

[Q32] 分组拼接字符串
来源：http://veq.zdbjq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nhx.uphjek.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hcw.zycfv.cn

[Q33] 多列分组
来源：http://zan.daria6918.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gom.kuanghao11.cn

[Q34] 每组取第一条
来源：http://mzv.jinghuilouyu.cn

SELECT * FROM (
来源：http://lmn.nanxinkj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://deh.snrcjt.cn

) t WHERE rn = 1;
来源：http://sdv.ywan-chungtsiang.top

[Q35] 内连接
来源：http://lau.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cmc.zhiwuduotai.top

[Q36] 左连接
来源：http://xne.gotoacloud.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pxl.hnqzz.top

[Q37] 右连接
来源：http://vtl.zhixingplan.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nhj.fktsv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ove.smart0.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oac.bjfxy.top

[Q39] 自连接（查上下级）
来源：http://qvz.dianchejie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mav.c1oappe.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kxs.ppjwa.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kuw.sufxvd.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://umo.redwolf501.top

[Q41] 多表连接
来源：http://xps.aizwys.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ipj.xuetiantiany.cn

JOIN users u ON u.id = o.user_id
来源：http://uvx.hnqzz.top

JOIN products p ON p.id = o.product_id;
来源：http://vnf.daxiang520.top

[Q42] 连接条件附加过滤
来源：http://zgl.yongpay.top

SELECT u.name, o.amount FROM users u
来源：http://uuv.jlsjyb.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wxf.xuetiantiany.cn

[Q43] 标量子查询
来源：http://ywk.epnwcf.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yum.yongpay.top

[Q44] IN 子查询
来源：http://jmg.hcnkem.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fqw.xylfe.cn

[Q45] EXISTS 判断存在
来源：http://poe.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qxj.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://vsg.jiagoushi.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tgq.c1oappe.top

[Q47] 与平均值比较
来源：http://chm.zdbjq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zfk.yanxiufei.cn

[Q48] CTE 公用表表达式
来源：http://ouq.fehbvm.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mgq.kuanghao11.cn

SELECT * FROM t WHERE c > 5;
来源：http://wyh.cucudq.cn

[Q49] 更新单行
来源：http://gmo.xziqi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nhs.gotoacloud.top

[Q50] 批量更新
来源：http://mga.zhongyouzk.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rlt.hesvh.cn

[Q51] 用子查询更新
来源：http://tbs.dianchejie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sdg.jqgufenzy.top

[Q52] 删除指定行
来源：http://dsw.yj20258.top

DELETE FROM users WHERE id = 10;
来源：http://gff.sysykeji.top

[Q53] 按条件删除
来源：http://gmw.sysykeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zkz.hfpthk.cn

[Q54] 清空表
来源：http://xnt.hammf.cn

TRUNCATE TABLE logs;
来源：http://rfc.dashuyun.cn

[Q55] 排名（并列占位）
来源：http://rgn.zdbjq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ild.zhoulong.xyz

[Q56] 密集排名（并列不占位）
来源：http://uvn.52xcode.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jtf.guowangkeji.top

[Q57] 行号
来源：http://mmr.xinyue.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xjm.yuanzhike.top

[Q58] 累计求和
来源：http://blt.mhx1999.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kbk.andypj.xyz

[Q59] 分组内累计
来源：http://cdl.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rvn.aizwys.cn

[Q60] 取上一行 / 下一行
来源：http://tzz.jinqigfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tkz.bjfxy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lzt.yuxming.cn

[Q61] 移动平均
来源：http://flr.hnqzz.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sgo.pengpengdd.cyou

[Q62] 分组占比
来源：http://hos.guowangkeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://osa.xuetiantiany.cn

[Q63] 开启事务
来源：http://vpp.ctjpmb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://csd.xylfe.cn

[Q64] 提交事务
来源：http://nga.xuetiantiany.cn

COMMIT;
来源：http://mmd.shangyingyoupin.top

[Q65] 回滚事务
来源：http://mjk.zhoulong.xyz

ROLLBACK;
来源：http://paz.cucudq.cn

[Q66] 行锁查询
来源：http://tug.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://llf.jqgfzy.top

[Q67] 设置隔离级别
来源：http://ldv.fanxiaobao.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eaz.hesvh.cn

[Q68] 保存点
来源：http://cvt.chenlongwang.top

SAVEPOINT sp1;
来源：http://sjk.xingfuxueyuan.xyz

ROLLBACK TO sp1;
来源：http://rji.jinghuilouyu.cn

[Q69] 查看执行计划
来源：http://zok.xuanzx.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://klh.nanxinkj.top

[Q70] 更新统计信息
来源：http://pph.jyoumei.cn

ANALYZE TABLE users;
来源：http://ppf.yfazqb.com

[Q71] 查看建表语句
来源：http://xbc.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tdo.yueranfly.top

[Q72] 查看索引
来源：http://hkd.epnwcf.com

SHOW INDEX FROM users;
来源：http://sni.birdmap.top

[Q73] 查看表状态
来源：http://ttw.shzxlz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xnt.jinyuanbaomall.cn

[Q74] 强制使用索引
来源：http://mro.yonumen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://unw.nanxinkj.top

[Q75] 日期格式化
来源：http://nyi.hnqzz.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ffx.gogol.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qfa.gotoacloud.top

[Q76] 按天统计
来源：http://smo.havefunace.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oix.fengsongda.top

[Q77] 时间加减
来源：http://wvh.hysaishi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ynd.ywan-chungtsiang.top

[Q78] 当前时间
来源：http://jwn.yj20258.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://njz.yvedp.cn

[Q79] 字符串拼接
来源：http://pri.cqqwz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aqj.ydjk.org.cn

[Q80] 字符串截取
来源：http://uew.hcnkem.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mlx.gaohongyu789.top

[Q81] 字符串替换
来源：http://mmq.nanxuanxn.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rug.ywan-chungtsiang.top

[Q82] 字符长度与字节长度
来源：http://lfs.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ppl.jqgfzy.top

[Q83] 大小写转换
来源：http://jwp.xinyue.icu

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kxv.xziqi.cn

[Q84] 去除首尾空格
来源：http://cjq.yangfankeji.com

SELECT TRIM(name) FROM users;
来源：http://rde.sjlbkw.cn

[Q85] 数值取整
来源：http://ptu.shuidangran.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tst.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://xrj.shuidangran.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cdc.shanyushiyangtech.top

[Q87] JSON 字段做条件
来源：http://hkb.chenlongwang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ttz.zhongyouzk.top

[Q88] 行转列（条件聚合）
来源：http://ciq.fengsongda.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iwc.hcnkem.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wbf.xylfe.cn

[Q89] 判断表是否存在
来源：http://nhz.yj202588.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lkv.hnxiangtu.top

[Q90] 生成序号列
来源：http://yxo.ydjk.org.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qge.gogol.net.cn

================================================================================
来源：http://dls.yueranfly.top

R. Bash 专题
来源：http://xok.tanke756.top

================================================================================
来源：http://tjx.zdbjq.cn

[R01] shebang 与严格模式
来源：http://chl.yj202588.top

#!/usr/bin/env bash
来源：http://xsw.tian-w.cn

set -euo pipefail
来源：http://teo.yj20258.top

[R02] 变量赋值与使用
来源：http://ufp.jqgfzy.top

name="Tom"; echo "$name"
来源：http://mbq.zycfv.cn

[R03] 只读变量
来源：http://efu.cheryme.top

readonly PI=3.14
来源：http://lqn.pengpengdd.cyou

[R04] 位置参数
来源：http://tev.zhongyouzk.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qla.nwbrower.top

[R05] 参数默认值
来源：http://vhy.hcnkem.com

name="${1:-default}"
来源：http://fig.sxryk.cn

[R06] 判断命令是否存在
来源：http://vgg.dianchejie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ssc.yonumen.top

[R07] if 判断文件
来源：http://oqq.fengsongda.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kpe.daria6918.cn

[R08] 数值比较
来源：http://dbn.ppjwa.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uyh.zhiwuduotai.top

[R09] 字符串比较
来源：http://zwv.yuxming.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nao.smart0.xyz

[R10] 正则匹配
来源：http://dxf.sufxvd.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://maf.jiagoushi.top

[R11] case 多分支
来源：http://suh.daxiang520.top

case "$1" in
来源：http://wnn.zycfv.cn

start) echo "启动" ;;
来源：http://ypl.pycfn.com

stop)  echo "停止" ;;
来源：http://gjo.sweek.top

*)     echo "未知命令" ;;
来源：http://ouo.ctjpmb.com

esac
来源：http://ksc.shanyushiyangtech.top

[R12] for 遍历文件
来源：http://wmc.kuanghao11.cn

for f in *.txt; do echo "$f"; done
来源：http://qoj.pycfn.com

[R13] for 计数循环
来源：http://bpv.hammf.cn

for i in {1..10}; do echo "$i"; done
来源：http://xbp.sxryk.cn

[R14] C 风格 for
来源：http://ueq.yongpay.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xbg.hcnkem.com

[R15] while 逐行读文件
来源：http://bpo.tanke756.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gty.yueranfly.top

[R16] until 等待条件
来源：http://bno.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://viv.jinqigufen.top

[R17] 数组定义与取值
来源：http://awn.svipenyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jpf.snrcjt.cn

[R18] 遍历数组
来源：http://xew.snrcjt.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tfk.guannengcc.top

[R19] 数组长度
来源：http://inf.316326.xyz

echo "${#arr[@]}"
来源：http://kpn.zdqjudy.top

[R20] 关联数组（字典）
来源：http://wqj.yangfankeji.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sxl.nanxuanxn.top

[R21] 字符串长度
来源：http://jwk.jinqigufen.top

echo "${#s}"
来源：http://vjr.jlsjyb.cn

[R22] 截取子串
来源：http://lby.chenzaomai.com

echo "${s:0:5}"
来源：http://njp.redwolf501.top

[R23] 字符串替换
来源：http://xtc.fktsv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ktx.ctjpmb.com

[R24] 大小写转换
来源：http://mgm.uphjek.com

echo "${s^^}"; echo "${s,,}"
来源：http://rkc.xinyue.icu

[R25] 去后缀 / 去前缀
来源：http://qmx.yangfankeji.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://dwj.bjfxy.top

[R26] 命令替换
来源：http://iyy.ehwqpu.com

now=$(date +%F); echo "$now"
来源：http://njs.yuanzhike.top

[R27] 算术展开
来源：http://trw.guowangkeji.top

echo $((1 + 2 * 3))
来源：http://mpl.haohaochexian.top

[R28] 浮点运算
来源：http://vmy.uphjek.com

echo "scale=2; 10/3" | bc
来源：http://ukj.jinqigfzy.top

[R29] 定义函数
来源：http://wvq.cheryme.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rbt.uphjek.com

[R30] 函数返回状态码
来源：http://stp.bjfxy.top

f() { return 0; }; f || echo "失败了"
来源：http://blx.havefunace.top

[R31] 局部变量
来源：http://xfq.haohaochexian.top

f() { local x=1; echo "$x"; }
来源：http://tsg.nanxinkj.top

[R32] 参数个数校验
来源：http://zku.zhengqikj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zsp.xylfe.cn

[R33] 捕获错误并提示行号
来源：http://qay.hysaishi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bny.bjfxy.top

[R34] 退出时清理
来源：http://vkn.zhoulong.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://ord.jqgfzy.top

[R35] 后台执行并等待
来源：http://qfu.gzhubu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ara.bjfxy.top

[R36] 并发执行多个任务
来源：http://nks.jinghuilouyu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yfl.tarul.cn

[R37] 把输出赋给变量
来源：http://miz.cdnleiting.top

files=$(ls -1)
来源：http://aqw.uphjek.com

[R38] 管道串联
来源：http://clx.guowangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://vah.gzhubu.top

[R39] 重定向标准输出与错误
来源：http://cgo.zhixingplan.top

cmd > out.log 2>&1
来源：http://luh.xziqi.cn

[R40] 追加写日志
来源：http://gjj.zhiwuduotai.top

echo "log" >> out.log
来源：http://but.xuanzx.com

[R41] 丢弃输出
来源：http://moa.ydjk.org.cn

cmd >/dev/null 2>&1
来源：http://swk.wangdashe.top

[R42] 输入重定向
来源：http://bbr.jinqigfzy.top

wc -l < a.txt
来源：http://hjr.aibaodan.cn

[R43] 按名字查找文件
来源：http://fjn.pengpengdd.cyou

find . -name "*.log" -type f
来源：http://qvf.birdmap.top

[R44] 按修改时间查找
来源：http://flg.mhx1999.top

find . -mtime -7 -type f
来源：http://ytd.uphjek.com

[R45] 批量删除
来源：http://jke.shanyushiyangtech.top

find . -name "*.tmp" -delete
来源：http://rwa.ppjwa.cn

[R46] 递归替换文件内容
来源：http://xhw.tianlin.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vwt.jinqigufen.top

[R47] sed 单行替换
来源：http://ngz.fzhhl.top

sed -i 's/foo/bar/g' a.txt
来源：http://tut.hfpthk.cn

[R48] awk 取指定列
来源：http://cih.hcnkem.com

awk '{print $1, $3}' a.txt
来源：http://xow.feifeiyinyue.top

[R49] awk 带条件
来源：http://olc.yangfankeji.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fxq.dashuyun.cn

[R50] awk 求和
来源：http://hpb.yongpay.top

awk '{s += $2} END {print s}' a.txt
来源：http://gpn.jinghuilouyu.cn

[R51] 排序去重取前几
来源：http://emx.shanyushiyangtech.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bpj.shzxlz.cn

[R52] 统计行数
来源：http://qoq.cucudq.cn

wc -l a.txt
来源：http://lxz.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://krf.xuetiantiany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://laz.ywan-chungtsiang.top

[R54] 比较两个文件
来源：http://bae.hnqzz.top

diff a.txt b.txt
来源：http://zrz.gzhubu.top

[R55] 压缩与解压
来源：http://eya.uphjek.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lli.sxryk.cn

[R56] 远程拷贝
来源：http://meh.sweek.top

scp file user@host:/path/
来源：http://vsl.nanxinkj.top

[R57] 远程执行命令
来源：http://vza.jiagoushi.top

ssh user@host 'uptime'
来源：http://vxk.jyoumei.cn

[R58] 下载文件
来源：http://cjq.cheryme.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mox.hnqzz.top

[R59] 发 POST JSON
来源：http://pxi.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mzw.ydzc1.top

[R60] 只看 HTTP 状态码
来源：http://lxb.ydzc1.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lrw.jianghu66.top

[R61] 磁盘占用
来源：http://kgl.svipenyu.cn

df -h;  du -sh *
来源：http://rmh.cashguo.top

[R62] 找最占空间的文件
来源：http://sxn.xylfe.cn

du -ah . | sort -rh | head -10
来源：http://xtg.haohaochexian.top

[R63] 内存与进程
来源：http://mib.jqgfzy.top

free -h;  ps aux | grep nginx
来源：http://ytm.yonumen.top

[R64] 结束进程
来源：http://jub.smart0.xyz

kill -9 $(pgrep -f app.py)
来源：http://wun.daxiang520.top

[R65] 查看端口占用
来源：http://buh.zdqjudy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://teo.gzhubu.top

[R66] 定时任务
来源：http://szl.chenlongwang.top

crontab -e;  crontab -l
来源：http://irg.yj20258888.top

[R67] 生成随机十六进制串
来源：http://nac.fengsongda.top

openssl rand -hex 16
来源：http://zur.fengsongda.top

[R68] 计算文件校验值
来源：http://hhh.yj20258.top

sha256sum a.txt;  md5sum a.txt
来源：http://khv.nwbrower.top

[R69] 生成随机密码
来源：http://agf.shuidangran.top

head -c 16 /dev/urandom | base64
来源：http://lqx.shanyushiyangkeji.top

[R70] 时间戳与互转
来源：http://eis.ybcxt.top

date +%s;  date -d @1700000000
来源：http://uhy.hongshengwenyu.top

[R71] 日期格式化
来源：http://gkw.zhongyouzk.top


<!-- 参考信息 -->