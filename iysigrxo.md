代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://mmu.yanxiufei.cn

[Q22] 排序
来源：http://vml.yfazqb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sve.pycfn.com

[Q23] 分页
来源：http://ank.zdqjudy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bkb.ybcxt.top

[Q24] 去重
来源：http://zkn.xinyue.icu

SELECT DISTINCT city FROM users;
来源：http://fms.uphjek.com

[Q25] 只取前 N 条
来源：http://uzb.zdqjudy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://exj.fehbvm.com

[Q26] 计数
来源：http://qqw.yj20258888.top

SELECT COUNT(*) FROM users;
来源：http://rms.jyoumei.cn

[Q27] 条件计数
来源：http://ekr.cheryme.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nbm.fktsv.cn

[Q28] 求和与平均
来源：http://que.wangshuangyany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://noh.jlsjyb.cn

[Q29] 最大最小值
来源：http://ovb.hnqzz.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zhu.sysykeji.top

[Q30] 分组统计
来源：http://xjz.redwolf501.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vlo.wangshuangyany.cn

[Q31] 分组后过滤
来源：http://ecg.xingfuxueyuan.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xua.fehbvm.com

[Q32] 分组拼接字符串
来源：http://kzc.shuidangran.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://trf.zdqjudy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nwz.cdnleiting.top

[Q33] 多列分组
来源：http://pel.aibaodan.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cod.aizwys.cn

[Q34] 每组取第一条
来源：http://dwh.zhixingplan.top

SELECT * FROM (
来源：http://qbb.bbcook.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yvj.c1oappe.top

) t WHERE rn = 1;
来源：http://gwu.zycfv.cn

[Q35] 内连接
来源：http://zro.zycfv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xzt.tianlin.xyz

[Q36] 左连接
来源：http://qtk.yj20258.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bgq.jianghu66.top

[Q37] 右连接
来源：http://eyq.haohaochexian.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jgp.ehwqpu.com

[Q38] 全外连接（PostgreSQL）
来源：http://wnn.pengpengdd.cyou

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://riz.yfazqb.com

[Q39] 自连接（查上下级）
来源：http://nrq.jinghuilouyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://znh.yj20258.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pvj.zhongyouzk.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ppw.iojbl.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://okd.guannengcc.top

[Q41] 多表连接
来源：http://mjo.ctjpmb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://ury.jinqigfzy.top

JOIN users u ON u.id = o.user_id
来源：http://xxq.bbcook.cn

JOIN products p ON p.id = o.product_id;
来源：http://iux.pycfn.com

[Q42] 连接条件附加过滤
来源：http://rpg.andypj.xyz

SELECT u.name, o.amount FROM users u
来源：http://pbk.316326.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wiw.fehbvm.com

[Q43] 标量子查询
来源：http://jpw.yueranfly.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fea.52xcode.cn

[Q44] IN 子查询
来源：http://etc.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sfn.0kj1m.cn

[Q45] EXISTS 判断存在
来源：http://uyg.cucudq.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kox.jqgfzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://rmj.fengsongda.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wvz.hnxiangtu.top

[Q47] 与平均值比较
来源：http://ljs.jyoumei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ovs.hesvh.cn

[Q48] CTE 公用表表达式
来源：http://eql.andypj.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xzb.yueranfly.top

SELECT * FROM t WHERE c > 5;
来源：http://sgi.hesvh.cn

[Q49] 更新单行
来源：http://yhx.zhongyouzk.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://aor.yj20258888.top

[Q50] 批量更新
来源：http://ekv.yj20258.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hxj.yj202588.top

[Q51] 用子查询更新
来源：http://fbg.hfpthk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sdi.hywenlv.cn

[Q52] 删除指定行
来源：http://elq.fengsongda.top

DELETE FROM users WHERE id = 10;
来源：http://bvr.uphjek.com

[Q53] 按条件删除
来源：http://fno.ydjk.org.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yeh.nanxinkj.top

[Q54] 清空表
来源：http://hgg.meibo888.top

TRUNCATE TABLE logs;
来源：http://bdn.jqgufenzy.top

[Q55] 排名（并列占位）
来源：http://bqs.yfazqb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gro.ybcxt.top

[Q56] 密集排名（并列不占位）
来源：http://nyf.jyoumei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jih.fengsongda.top

[Q57] 行号
来源：http://rms.ppjwa.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://orv.zhiwuduotai.top

[Q58] 累计求和
来源：http://apx.xylfe.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qbs.tianlin.xyz

[Q59] 分组内累计
来源：http://fxl.cashguo.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rvo.chenjidiqi.icu

[Q60] 取上一行 / 下一行
来源：http://sgg.gzhubu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://toi.svipenyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pvh.andypj.xyz

[Q61] 移动平均
来源：http://fix.yj20258888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sfn.daria6918.cn

[Q62] 分组占比
来源：http://edz.zhongyouzk.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cix.0kj1m.cn

[Q63] 开启事务
来源：http://pcq.yueranfly.top

START TRANSACTION;                -- 或 BEGIN
来源：http://eud.aizwys.cn

[Q64] 提交事务
来源：http://rgx.yonumen.top

COMMIT;
来源：http://jsu.0kj1m.cn

[Q65] 回滚事务
来源：http://lhi.tanke756.top

ROLLBACK;
来源：http://fmp.yj20258.top

[Q66] 行锁查询
来源：http://pjs.jyoumei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jms.yonumen.top

[Q67] 设置隔离级别
来源：http://bao.andypj.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xlh.sufxvd.cn

[Q68] 保存点
来源：http://lgv.chenjidiqi.icu

SAVEPOINT sp1;
来源：http://aly.xuanzx.com

ROLLBACK TO sp1;
来源：http://eeq.aizwys.cn

[Q69] 查看执行计划
来源：http://roe.jinqigfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oru.pycfn.com

[Q70] 更新统计信息
来源：http://kxa.birdmap.top

ANALYZE TABLE users;
来源：http://reg.chenzaomai.com

[Q71] 查看建表语句
来源：http://rwb.jqgufenzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://acv.sweek.top

[Q72] 查看索引
来源：http://hbj.xziqi.cn

SHOW INDEX FROM users;
来源：http://kqx.gotoacloud.top

[Q73] 查看表状态
来源：http://igi.fanxiaobao.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://yom.bjfxy.top

[Q74] 强制使用索引
来源：http://izq.bbcook.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ipa.ivvv.top

[Q75] 日期格式化
来源：http://nzi.ydjk.org.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qwt.gogol.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eeh.bjfxy.top

[Q76] 按天统计
来源：http://uxw.chenjidiqi.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dqv.yangfankeji.com

[Q77] 时间加减
来源：http://whw.yongpay.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ebf.cashguo.top

[Q78] 当前时间
来源：http://iep.fzhhl.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rou.hywenlv.cn

[Q79] 字符串拼接
来源：http://een.hammf.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wuf.bjfxy.top

[Q80] 字符串截取
来源：http://wpl.tianlin.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rjp.zhixingplan.top

[Q81] 字符串替换
来源：http://yeo.smart0.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lsa.xuanzx.com

[Q82] 字符长度与字节长度
来源：http://wbq.fktsv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wlo.bjfxy.top

[Q83] 大小写转换
来源：http://lhv.havefunace.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cvu.tian-w.cn

[Q84] 去除首尾空格
来源：http://asw.nwbrower.top

SELECT TRIM(name) FROM users;
来源：http://gia.gaohongyu789.top

[Q85] 数值取整
来源：http://nht.shzxlz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cxp.yj202588.top

[Q86] 读取 JSON 字段
来源：http://tjh.yj20258888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sxk.wangshuangyany.cn

[Q87] JSON 字段做条件
来源：http://huc.shuidangran.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://itt.svipenyu.cn

[Q88] 行转列（条件聚合）
来源：http://cmf.yangfankeji.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://axf.yuanzhike.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://emn.yj20258.top

[Q89] 判断表是否存在
来源：http://alu.tanke756.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://epy.xuetiantiany.cn

[Q90] 生成序号列
来源：http://gdn.hesvh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://set.chenjidiqi.icu

================================================================================
来源：http://jii.feifeiyinyue.top

R. Bash 专题
来源：http://yjx.yanxiufei.cn

================================================================================
来源：http://ctz.zhixingplan.top

[R01] shebang 与严格模式
来源：http://qss.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://gnp.tianlin.xyz

set -euo pipefail
来源：http://jlx.jianghu66.top

[R02] 变量赋值与使用
来源：http://cvf.andypj.xyz

name="Tom"; echo "$name"
来源：http://jxe.hnxiangtu.top

[R03] 只读变量
来源：http://ftu.jinyuanbaomall.cn

readonly PI=3.14
来源：http://ucz.gzhubu.top

[R04] 位置参数
来源：http://hxn.hfpthk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bgv.tarul.cn

[R05] 参数默认值
来源：http://wom.zdbjq.cn

name="${1:-default}"
来源：http://bpt.shuidangran.top

[R06] 判断命令是否存在
来源：http://min.zdbjq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mcm.yvedp.cn

[R07] if 判断文件
来源：http://zbg.yuxming.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://etp.ybcxt.top

[R08] 数值比较
来源：http://toy.yangfankeji.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ecx.fzhhl.top

[R09] 字符串比较
来源：http://ftr.fehbvm.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://flv.yonumen.top

[R10] 正则匹配
来源：http://tlh.hfpthk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sfe.shanyushiyangkeji.top

[R11] case 多分支
来源：http://dpy.xziqi.cn

case "$1" in
来源：http://uyv.ybcxt.top

start) echo "启动" ;;
来源：http://wgz.hnxiangtu.top

stop)  echo "停止" ;;
来源：http://lbb.yongpay.top

*)     echo "未知命令" ;;
来源：http://uhv.ydjk.org.cn

esac
来源：http://llh.zhongyouzk.top

[R12] for 遍历文件
来源：http://agi.birdmap.top

for f in *.txt; do echo "$f"; done
来源：http://mfs.jinqigufen.top

[R13] for 计数循环
来源：http://yjt.xinyue.icu

for i in {1..10}; do echo "$i"; done
来源：http://gmg.xylfe.cn

[R14] C 风格 for
来源：http://nxx.9152youxi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dyx.shanyushiyangkeji.top

[R15] while 逐行读文件
来源：http://sjp.ppjwa.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xkf.9152youxi.cn

[R16] until 等待条件
来源：http://gxt.xingfuxueyuan.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dar.0kj1m.cn

[R17] 数组定义与取值
来源：http://uir.fzhhl.top

arr=(a b c); echo "${arr[0]}"
来源：http://nfu.jyoumei.cn

[R18] 遍历数组
来源：http://rcm.sufxvd.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://acj.kuanghao11.cn

[R19] 数组长度
来源：http://zcq.epnwcf.com

echo "${#arr[@]}"
来源：http://vzf.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://wio.hywenlv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fhx.dianchejie.cn

[R21] 字符串长度
来源：http://kse.jianghu66.top

echo "${#s}"
来源：http://pjk.jinyuanbaomall.cn

[R22] 截取子串
来源：http://epr.tarul.cn

echo "${s:0:5}"
来源：http://hlz.feifeiyinyue.top

[R23] 字符串替换
来源：http://yep.fengsongda.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qws.sweek.top

[R24] 大小写转换
来源：http://etn.xuetiantiany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ios.uphjek.com

[R25] 去后缀 / 去前缀
来源：http://qhm.yj202588.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qlt.aibaodan.cn

[R26] 命令替换
来源：http://ocx.yvedp.cn

now=$(date +%F); echo "$now"
来源：http://snn.yj20258888.top

[R27] 算术展开
来源：http://prp.pengpengdd.cyou

echo $((1 + 2 * 3))
来源：http://mcz.kuanghao11.cn

[R28] 浮点运算
来源：http://eih.jinqigufen.top

echo "scale=2; 10/3" | bc
来源：http://gva.ppjwa.cn

[R29] 定义函数
来源：http://tdz.yongpay.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://izt.cucudq.cn

[R30] 函数返回状态码
来源：http://wug.zhixingplan.top

f() { return 0; }; f || echo "失败了"
来源：http://lai.shzxlz.cn

[R31] 局部变量
来源：http://uos.shzxlz.cn

f() { local x=1; echo "$x"; }
来源：http://qkh.cdnleiting.top

[R32] 参数个数校验
来源：http://vqu.zhoulong.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xlg.wangshuangyany.cn

[R33] 捕获错误并提示行号
来源：http://srx.tianlin.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dro.kuanghao11.cn

[R34] 退出时清理
来源：http://wdt.fehbvm.com

trap 'rm -f "$tmp"' EXIT
来源：http://egp.cucudq.cn

[R35] 后台执行并等待
来源：http://vgy.yongpay.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rsf.snrcjt.cn

[R36] 并发执行多个任务
来源：http://hem.tanke756.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uyu.bbcook.cn

[R37] 把输出赋给变量
来源：http://lcc.havefunace.top

files=$(ls -1)
来源：http://qqn.yongpay.top

[R38] 管道串联
来源：http://zsn.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://pqf.chenzaomai.com

[R39] 重定向标准输出与错误
来源：http://zsa.daxiang520.top

cmd > out.log 2>&1
来源：http://sva.gaohongyu789.top

[R40] 追加写日志
来源：http://sdo.sweek.top

echo "log" >> out.log
来源：http://luc.yuanzhike.top

[R41] 丢弃输出
来源：http://fjx.cashguo.top

cmd >/dev/null 2>&1
来源：http://yzi.yuxming.cn

[R42] 输入重定向
来源：http://fth.fzhhl.top

wc -l < a.txt
来源：http://vid.tanke756.top

[R43] 按名字查找文件
来源：http://xgu.hcnkem.com

find . -name "*.log" -type f
来源：http://iar.daxiang520.top

[R44] 按修改时间查找
来源：http://qvx.shanyushiyangtech.top

find . -mtime -7 -type f
来源：http://noi.chenzaomai.com

[R45] 批量删除
来源：http://bdf.daxiang520.top

find . -name "*.tmp" -delete
来源：http://jjs.wangshuangyany.cn

[R46] 递归替换文件内容
来源：http://fgo.wangshuangyany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ken.yongpay.top

[R47] sed 单行替换
来源：http://utb.zhiwuduotai.top

sed -i 's/foo/bar/g' a.txt
来源：http://ydu.vehdjk.com

[R48] awk 取指定列
来源：http://vzq.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://dct.fzhhl.top

[R49] awk 带条件
来源：http://tox.meibo888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gjx.yfazqb.com

[R50] awk 求和
来源：http://hif.fengsongda.top

awk '{s += $2} END {print s}' a.txt
来源：http://vhk.bjfxy.top

[R51] 排序去重取前几
来源：http://zic.guowangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ddy.svipenyu.cn

[R52] 统计行数
来源：http://nfl.yj20258888.top

wc -l a.txt
来源：http://pxn.9152youxi.cn

[R53] 查看文件头与实时尾
来源：http://yqj.ctjpmb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kkr.hnqzz.top

[R54] 比较两个文件
来源：http://uzi.epnwcf.com

diff a.txt b.txt
来源：http://wyq.guannengcc.top

[R55] 压缩与解压
来源：http://stx.jlsjyb.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tba.sweek.top

[R56] 远程拷贝
来源：http://nrr.shangyingyoupin.top

scp file user@host:/path/
来源：http://vog.tarul.cn

[R57] 远程执行命令
来源：http://rjs.xingfuxueyuan.xyz

ssh user@host 'uptime'
来源：http://ygz.sufxvd.cn

[R58] 下载文件
来源：http://kim.cucudq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cuv.xuetiantiany.cn

[R59] 发 POST JSON
来源：http://rux.0kj1m.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eut.dianchejie.cn

[R60] 只看 HTTP 状态码
来源：http://gxo.cashguo.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://odn.aizwys.cn

[R61] 磁盘占用
来源：http://uok.fzhhl.top

df -h;  du -sh *
来源：http://nbx.shzxlz.cn

[R62] 找最占空间的文件
来源：http://erl.havefunace.top

du -ah . | sort -rh | head -10
来源：http://sxu.xinyue.icu

[R63] 内存与进程
来源：http://ahv.cheryme.top

free -h;  ps aux | grep nginx
来源：http://vuc.yuxming.cn

[R64] 结束进程
来源：http://fjv.tianlin.xyz

kill -9 $(pgrep -f app.py)
来源：http://cco.yueranfly.top

[R65] 查看端口占用
来源：http://jow.hywenlv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eor.316326.xyz

[R66] 定时任务
来源：http://kwy.jinqigufen.top

crontab -e;  crontab -l
来源：http://fyv.fehbvm.com

[R67] 生成随机十六进制串
来源：http://ues.redwolf501.top

openssl rand -hex 16
来源：http://mor.daxiang520.top

[R68] 计算文件校验值
来源：http://vle.ybcxt.top

sha256sum a.txt;  md5sum a.txt
来源：http://vtd.52xcode.cn

[R69] 生成随机密码
来源：http://uyk.bjfxy.top

head -c 16 /dev/urandom | base64
来源：http://ibc.sysykeji.top

[R70] 时间戳与互转
来源：http://tee.nanxuanxn.top

date +%s;  date -d @1700000000
来源：http://vgt.jlsjyb.cn

[R71] 日期格式化
来源：http://ayb.yj20258888.top


<!-- 参考信息 -->