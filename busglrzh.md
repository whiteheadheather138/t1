代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mhk.yueranfly.top

[Q20] IN 列表
来源：http://xew.9152youxi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sct.jinghuilouyu.cn

[Q21] 空值判断
来源：http://kak.fehbvm.com

SELECT * FROM users WHERE email IS NULL;
来源：http://qty.shangyingyoupin.top

[Q22] 排序
来源：http://agp.hnqzz.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ijg.sysykeji.top

[Q23] 分页
来源：http://hra.chenlongwang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wuu.bjfxy.top

[Q24] 去重
来源：http://hwv.zhengqikj.top

SELECT DISTINCT city FROM users;
来源：http://mcq.jiagoushi.top

[Q25] 只取前 N 条
来源：http://zxc.zhixingplan.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oep.zdbjq.cn

[Q26] 计数
来源：http://xfb.ctjpmb.com

SELECT COUNT(*) FROM users;
来源：http://cyi.cqqwz.cn

[Q27] 条件计数
来源：http://vci.hcnkem.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hrq.jqgufenzy.top

[Q28] 求和与平均
来源：http://hkz.xuetiantiany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ysq.tian-w.cn

[Q29] 最大最小值
来源：http://acq.yfazqb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://bva.zhengqikj.top

[Q30] 分组统计
来源：http://eyo.52xcode.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vvp.fanxiaobao.xyz

[Q31] 分组后过滤
来源：http://jyc.epnwcf.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ngk.aibaodan.cn

[Q32] 分组拼接字符串
来源：http://uln.nanxinkj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gla.dashuyun.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nrw.nanxinkj.top

[Q33] 多列分组
来源：http://rrx.yfazqb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tuf.hfpthk.cn

[Q34] 每组取第一条
来源：http://qwn.cqqwz.cn

SELECT * FROM (
来源：http://hia.yvedp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wjl.epnwcf.com

) t WHERE rn = 1;
来源：http://lkx.wangshuangyany.cn

[Q35] 内连接
来源：http://euu.nanxinkj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xqq.kuanghao11.cn

[Q36] 左连接
来源：http://nvu.yanxiufei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cib.pycfn.com

[Q37] 右连接
来源：http://vbp.uphjek.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kvz.wangdashe.top

[Q38] 全外连接（PostgreSQL）
来源：http://yle.feifeiyinyue.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lgj.pycfn.com

[Q39] 自连接（查上下级）
来源：http://aii.pycfn.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://fjk.quarkkingdee.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nlp.bjfxy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xsr.zhijiandao.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dlm.yj20258888.top

[Q41] 多表连接
来源：http://byw.pengpengdd.cyou

SELECT o.id, u.name, p.title FROM orders o
来源：http://uvp.jyoumei.cn

JOIN users u ON u.id = o.user_id
来源：http://uzu.hnxiangtu.top

JOIN products p ON p.id = o.product_id;
来源：http://rms.gogol.net.cn

[Q42] 连接条件附加过滤
来源：http://lnk.jyoumei.cn

SELECT u.name, o.amount FROM users u
来源：http://mrl.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hjk.jiagoushi.top

[Q43] 标量子查询
来源：http://zka.sysykeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xor.hywenlv.cn

[Q44] IN 子查询
来源：http://lip.tianlin.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vhi.daria6918.cn

[Q45] EXISTS 判断存在
来源：http://nlj.pycfn.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ktd.quarkkingdee.top

[Q46] NOT EXISTS 判断不存在
来源：http://mzn.xinyue.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ivg.guannengcc.top

[Q47] 与平均值比较
来源：http://ynv.hnxiangtu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gxj.smart0.xyz

[Q48] CTE 公用表表达式
来源：http://swc.dashuyun.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lgy.jlsjyb.cn

SELECT * FROM t WHERE c > 5;
来源：http://kup.yangfankeji.com

[Q49] 更新单行
来源：http://dcc.ydjk.org.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://akh.smart0.xyz

[Q50] 批量更新
来源：http://noy.shanyushiyangkeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tpk.52xcode.cn

[Q51] 用子查询更新
来源：http://hlq.uphjek.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sfz.xingfuxueyuan.xyz

[Q52] 删除指定行
来源：http://iba.xuanzx.com

DELETE FROM users WHERE id = 10;
来源：http://ejb.feifeiyinyue.top

[Q53] 按条件删除
来源：http://ifh.haohaochexian.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jej.havefunace.top

[Q54] 清空表
来源：http://nvl.sweek.top

TRUNCATE TABLE logs;
来源：http://udz.jqgfzy.top

[Q55] 排名（并列占位）
来源：http://cem.hnxiangtu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rdf.fzhhl.top

[Q56] 密集排名（并列不占位）
来源：http://nrt.dashuyun.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://piq.pycfn.com

[Q57] 行号
来源：http://dev.daxiang520.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ekb.fanxiaobao.xyz

[Q58] 累计求和
来源：http://bws.zhongyouzk.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jyt.hywenlv.cn

[Q59] 分组内累计
来源：http://uwf.ybcxt.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fef.yfazqb.com

[Q60] 取上一行 / 下一行
来源：http://puu.0kj1m.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aym.jlsjyb.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pmv.xylfe.cn

[Q61] 移动平均
来源：http://kjn.cashguo.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gsf.zycfv.cn

[Q62] 分组占比
来源：http://spw.shzxlz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://day.feifeiyinyue.top

[Q63] 开启事务
来源：http://keu.jianghu66.top

START TRANSACTION;                -- 或 BEGIN
来源：http://lfc.aibaodan.cn

[Q64] 提交事务
来源：http://kij.cucudq.cn

COMMIT;
来源：http://nrr.52xcode.cn

[Q65] 回滚事务
来源：http://gvc.cucudq.cn

ROLLBACK;
来源：http://tlz.tian-w.cn

[Q66] 行锁查询
来源：http://axt.ctjpmb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pou.shzxlz.cn

[Q67] 设置隔离级别
来源：http://sug.ctjpmb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pxf.ydjk.org.cn

[Q68] 保存点
来源：http://gks.zdqjudy.top

SAVEPOINT sp1;
来源：http://cvv.jyoumei.cn

ROLLBACK TO sp1;
来源：http://oxy.cheryme.top

[Q69] 查看执行计划
来源：http://mur.meibo888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nvu.hysaishi.cn

[Q70] 更新统计信息
来源：http://jyj.zhixingplan.top

ANALYZE TABLE users;
来源：http://gry.bbcook.cn

[Q71] 查看建表语句
来源：http://nzc.hywenlv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xbk.bjfxy.top

[Q72] 查看索引
来源：http://ike.zhaomingkeji.xyz

SHOW INDEX FROM users;
来源：http://lxn.jinghuilouyu.cn

[Q73] 查看表状态
来源：http://guy.cdnleiting.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rqo.hongshengwenyu.top

[Q74] 强制使用索引
来源：http://leb.xziqi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://esd.jinghuilouyu.cn

[Q75] 日期格式化
来源：http://njv.zhixingplan.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yvr.yvedp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yol.zdbjq.cn

[Q76] 按天统计
来源：http://brd.hcnkem.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ucr.gogol.net.cn

[Q77] 时间加减
来源：http://cvl.yangfankeji.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tmq.xingfuxueyuan.xyz

[Q78] 当前时间
来源：http://gel.shanyushiyangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ccd.9152youxi.cn

[Q79] 字符串拼接
来源：http://wip.cdnleiting.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ukg.yj20258888.top

[Q80] 字符串截取
来源：http://wjl.xuetiantiany.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nft.fanxiaobao.xyz

[Q81] 字符串替换
来源：http://pym.kuanghao11.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wwg.zhengqikj.top

[Q82] 字符长度与字节长度
来源：http://qtd.jianghu66.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yfh.havefunace.top

[Q83] 大小写转换
来源：http://nuy.wangshuangyany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zeo.chenlongwang.top

[Q84] 去除首尾空格
来源：http://gdz.sjlbkw.cn

SELECT TRIM(name) FROM users;
来源：http://rwv.ydjk.org.cn

[Q85] 数值取整
来源：http://weu.xingfuxueyuan.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sin.aibaodan.cn

[Q86] 读取 JSON 字段
来源：http://eci.uphjek.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hkx.bbcook.cn

[Q87] JSON 字段做条件
来源：http://frl.fzhhl.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://orh.tarul.cn

[Q88] 行转列（条件聚合）
来源：http://nrt.fanxiaobao.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eiv.shangyingyoupin.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nmz.yj20258888.top

[Q89] 判断表是否存在
来源：http://nlm.gogol.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://asf.0kj1m.cn

[Q90] 生成序号列
来源：http://gsf.ybcxt.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vut.hnxiangtu.top

================================================================================
来源：http://aus.ybcxt.top

R. Bash 专题
来源：http://ocn.yueranfly.top

================================================================================
来源：http://wdp.hfpthk.cn

[R01] shebang 与严格模式
来源：http://dov.zhongyouzk.top

#!/usr/bin/env bash
来源：http://pta.fehbvm.com

set -euo pipefail
来源：http://fkp.shangyingyoupin.top

[R02] 变量赋值与使用
来源：http://hyt.vqdsnc.cn

name="Tom"; echo "$name"
来源：http://dsd.jinqigufen.top

[R03] 只读变量
来源：http://uiv.cucudq.cn

readonly PI=3.14
来源：http://cub.haohaochexian.top

[R04] 位置参数
来源：http://vgr.pycfn.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pgd.svipenyu.cn

[R05] 参数默认值
来源：http://mjb.bjfxy.top

name="${1:-default}"
来源：http://lap.zhijiandao.cn

[R06] 判断命令是否存在
来源：http://kcz.gogol.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://drd.hnxiangtu.top

[R07] if 判断文件
来源：http://cgu.jyoumei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ogg.dashuyun.cn

[R08] 数值比较
来源：http://pco.quarkkingdee.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nte.zhixingplan.top

[R09] 字符串比较
来源：http://puf.mhx1999.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jmi.yj202588.top

[R10] 正则匹配
来源：http://umh.kuanghao11.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kun.cheryme.top

[R11] case 多分支
来源：http://szl.yj20258.top

case "$1" in
来源：http://txa.zhixingplan.top

start) echo "启动" ;;
来源：http://oaa.shangyingyoupin.top

stop)  echo "停止" ;;
来源：http://qur.tarul.cn

*)     echo "未知命令" ;;
来源：http://zpe.pycfn.com

esac
来源：http://glr.zhijiandao.cn

[R12] for 遍历文件
来源：http://bje.shzxlz.cn

for f in *.txt; do echo "$f"; done
来源：http://cmz.ydjk.org.cn

[R13] for 计数循环
来源：http://qza.shangyingyoupin.top

for i in {1..10}; do echo "$i"; done
来源：http://xpw.sjlbkw.cn

[R14] C 风格 for
来源：http://fer.ybcxt.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uie.shangyingyoupin.top

[R15] while 逐行读文件
来源：http://ukr.ywan-chungtsiang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tvv.yueranfly.top

[R16] until 等待条件
来源：http://kuv.yj202588.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yry.iojbl.cn

[R17] 数组定义与取值
来源：http://ebn.fanxiaobao.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://olm.dashuyun.cn

[R18] 遍历数组
来源：http://nai.aizwys.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pnc.xylfe.cn

[R19] 数组长度
来源：http://opu.guowangkeji.top

echo "${#arr[@]}"
来源：http://zgk.snrcjt.cn

[R20] 关联数组（字典）
来源：http://kfp.chenjidiqi.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kun.ctjpmb.com

[R21] 字符串长度
来源：http://qlu.sxryk.cn

echo "${#s}"
来源：http://ilx.fengsongda.top

[R22] 截取子串
来源：http://qll.haohaochexian.top

echo "${s:0:5}"
来源：http://baa.xinyue.icu

[R23] 字符串替换
来源：http://lde.chenjidiqi.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://efe.cucudq.cn

[R24] 大小写转换
来源：http://rjh.epnwcf.com

echo "${s^^}"; echo "${s,,}"
来源：http://dfv.zhengqikj.top

[R25] 去后缀 / 去前缀
来源：http://lxc.sjlbkw.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hjz.zdbjq.cn

[R26] 命令替换
来源：http://yao.quarkkingdee.top

now=$(date +%F); echo "$now"
来源：http://zhu.zdqjudy.top

[R27] 算术展开
来源：http://hrc.birdmap.top

echo $((1 + 2 * 3))
来源：http://gqd.sufxvd.cn

[R28] 浮点运算
来源：http://knh.ydzc1.top

echo "scale=2; 10/3" | bc
来源：http://fna.jianghu66.top

[R29] 定义函数
来源：http://qit.chenzaomai.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yrm.sjlbkw.cn

[R30] 函数返回状态码
来源：http://zbi.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://hoc.hcnkem.com

[R31] 局部变量
来源：http://ydb.jyoumei.cn

f() { local x=1; echo "$x"; }
来源：http://afa.xziqi.cn

[R32] 参数个数校验
来源：http://rtx.birdmap.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aks.tian-w.cn

[R33] 捕获错误并提示行号
来源：http://pdt.zhijiandao.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ige.dianchejie.cn

[R34] 退出时清理
来源：http://xgg.vehdjk.com

trap 'rm -f "$tmp"' EXIT
来源：http://zvy.pycfn.com

[R35] 后台执行并等待
来源：http://pst.ehwqpu.com

sleep 5 & pid=$!; wait "$pid"
来源：http://boa.52xcode.cn

[R36] 并发执行多个任务
来源：http://niw.daria6918.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qdv.hammf.cn

[R37] 把输出赋给变量
来源：http://zos.uphjek.com

files=$(ls -1)
来源：http://jds.vqdsnc.cn

[R38] 管道串联
来源：http://uxd.mhx1999.top

cat a.txt | grep -i error | wc -l
来源：http://sio.zhixingplan.top

[R39] 重定向标准输出与错误
来源：http://nrp.andypj.xyz

cmd > out.log 2>&1
来源：http://ovo.yuanzhike.top

[R40] 追加写日志
来源：http://ncu.andypj.xyz

echo "log" >> out.log
来源：http://ohg.wangshuangyany.cn

[R41] 丢弃输出
来源：http://rrq.yvedp.cn

cmd >/dev/null 2>&1
来源：http://ksc.bbcook.cn

[R42] 输入重定向
来源：http://lxp.pengpengdd.cyou

wc -l < a.txt
来源：http://ezh.zycfv.cn

[R43] 按名字查找文件
来源：http://kfo.chenlongwang.top

find . -name "*.log" -type f
来源：http://nki.jyoumei.cn

[R44] 按修改时间查找
来源：http://mwy.hcnkem.com

find . -mtime -7 -type f
来源：http://qrf.birdmap.top

[R45] 批量删除
来源：http://ivt.daria6918.cn

find . -name "*.tmp" -delete
来源：http://vgk.yangfankeji.com

[R46] 递归替换文件内容
来源：http://xml.zhoulong.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bsr.chenzaomai.com

[R47] sed 单行替换
来源：http://xwa.gzhubu.top

sed -i 's/foo/bar/g' a.txt
来源：http://yag.zhiwuduotai.top

[R48] awk 取指定列
来源：http://ogd.xingfuxueyuan.xyz

awk '{print $1, $3}' a.txt
来源：http://kpp.zhoulong.xyz

[R49] awk 带条件
来源：http://byd.hongshengwenyu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mza.gaohongyu789.top

[R50] awk 求和
来源：http://xey.bjfxy.top

awk '{s += $2} END {print s}' a.txt
来源：http://pyl.quarkkingdee.top

[R51] 排序去重取前几
来源：http://zed.tarul.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://emb.vqdsnc.cn

[R52] 统计行数
来源：http://fuj.hammf.cn

wc -l a.txt
来源：http://ebr.tanke756.top

[R53] 查看文件头与实时尾
来源：http://hla.guannengcc.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xgv.smart0.xyz

[R54] 比较两个文件
来源：http://jay.bbcook.cn

diff a.txt b.txt
来源：http://pbj.cheryme.top

[R55] 压缩与解压
来源：http://mox.yj202588.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xkq.zhoulong.xyz

[R56] 远程拷贝
来源：http://ofs.yongpay.top

scp file user@host:/path/
来源：http://rpz.yuxming.cn

[R57] 远程执行命令
来源：http://cdg.fktsv.cn

ssh user@host 'uptime'
来源：http://kvo.nwbrower.top

[R58] 下载文件
来源：http://zgn.feifeiyinyue.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ayl.gaohongyu789.top

[R59] 发 POST JSON
来源：http://wbu.chenlongwang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lka.ywan-chungtsiang.top

[R60] 只看 HTTP 状态码
来源：http://ulm.cucudq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://byt.fehbvm.com

[R61] 磁盘占用
来源：http://voq.hcnkem.com

df -h;  du -sh *
来源：http://tka.fzhhl.top

[R62] 找最占空间的文件
来源：http://mun.fengsongda.top

du -ah . | sort -rh | head -10
来源：http://sod.daxiang520.top

[R63] 内存与进程
来源：http://vjb.chenjidiqi.icu

free -h;  ps aux | grep nginx
来源：http://upl.feifeiyinyue.top

[R64] 结束进程
来源：http://obr.zhaomingkeji.xyz

kill -9 $(pgrep -f app.py)
来源：http://lge.hongshengwenyu.top

[R65] 查看端口占用
来源：http://jzn.fehbvm.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://krf.shanyushiyangkeji.top

[R66] 定时任务
来源：http://ihk.mhx1999.top

crontab -e;  crontab -l
来源：http://zdu.mhx1999.top

[R67] 生成随机十六进制串
来源：http://pyv.mhx1999.top

openssl rand -hex 16
来源：http://tlo.epnwcf.com

[R68] 计算文件校验值
来源：http://xsz.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hhq.xylfe.cn

[R69] 生成随机密码
来源：http://glm.shanyushiyangkeji.top


<!-- 参考信息 -->