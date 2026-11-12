代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ffd.sxryk.cn

[Q24] 去重
来源：http://ujl.redwolf501.top

SELECT DISTINCT city FROM users;
来源：http://wsh.feifeiyinyue.top

[Q25] 只取前 N 条
来源：http://hbv.yangfankeji.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nkt.ydzc1.top

[Q26] 计数
来源：http://sld.dashuyun.cn

SELECT COUNT(*) FROM users;
来源：http://nqm.zhijiandao.cn

[Q27] 条件计数
来源：http://lqd.jlsjyb.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jts.bjfxy.top

[Q28] 求和与平均
来源：http://jem.jqgfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qpz.yueranfly.top

[Q29] 最大最小值
来源：http://roc.hysaishi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gzv.aibaodan.cn

[Q30] 分组统计
来源：http://bwx.meibo888.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pkq.gaohongyu789.top

[Q31] 分组后过滤
来源：http://ddo.fengsongda.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kgv.epnwcf.com

[Q32] 分组拼接字符串
来源：http://egi.wangshuangyany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mat.ehwqpu.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rzr.yongpay.top

[Q33] 多列分组
来源：http://gdk.c1oappe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wsk.chenlongwang.top

[Q34] 每组取第一条
来源：http://jty.yfazqb.com

SELECT * FROM (
来源：http://ozm.iojbl.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nyo.yangfankeji.com

) t WHERE rn = 1;
来源：http://xld.pengpengdd.cyou

[Q35] 内连接
来源：http://rfi.gaohongyu789.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mkn.nanxuanxn.top

[Q36] 左连接
来源：http://ajj.xziqi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cmh.birdmap.top

[Q37] 右连接
来源：http://ykt.cheryme.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lor.jinqigfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://bzj.sufxvd.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ryj.ywan-chungtsiang.top

[Q39] 自连接（查上下级）
来源：http://tda.tanke756.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://acb.hfpthk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mvr.jqgfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fnn.hnqzz.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hjf.zycfv.cn

[Q41] 多表连接
来源：http://xkg.tarul.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://srj.yongpay.top

JOIN users u ON u.id = o.user_id
来源：http://qdx.xuetiantiany.cn

JOIN products p ON p.id = o.product_id;
来源：http://nak.xingfuxueyuan.xyz

[Q42] 连接条件附加过滤
来源：http://vwc.fzhhl.top

SELECT u.name, o.amount FROM users u
来源：http://vzg.jqgfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qus.ydjk.org.cn

[Q43] 标量子查询
来源：http://zff.yongpay.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pbq.svipenyu.cn

[Q44] IN 子查询
来源：http://rfg.nanxuanxn.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zel.gogol.net.cn

[Q45] EXISTS 判断存在
来源：http://pwu.hfpthk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://evc.iojbl.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ckn.cucudq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://onw.shzxlz.cn

[Q47] 与平均值比较
来源：http://pfp.yj20258888.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rhm.fanxiaobao.xyz

[Q48] CTE 公用表表达式
来源：http://zmv.jinyuanbaomall.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hdz.havefunace.top

SELECT * FROM t WHERE c > 5;
来源：http://edn.sufxvd.cn

[Q49] 更新单行
来源：http://cvb.yueranfly.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oum.hnxiangtu.top

[Q50] 批量更新
来源：http://gxt.haohaochexian.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kbz.hnqzz.top

[Q51] 用子查询更新
来源：http://wfq.havefunace.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hzp.wangshuangyany.cn

[Q52] 删除指定行
来源：http://tcd.hcnkem.com

DELETE FROM users WHERE id = 10;
来源：http://tgq.52xcode.cn

[Q53] 按条件删除
来源：http://jxg.sweek.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cnz.yj20258.top

[Q54] 清空表
来源：http://rsm.epnwcf.com

TRUNCATE TABLE logs;
来源：http://iyb.zhengqikj.top

[Q55] 排名（并列占位）
来源：http://dzu.aibaodan.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oos.xinyue.icu

[Q56] 密集排名（并列不占位）
来源：http://tvm.svipenyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rgz.ivvv.top

[Q57] 行号
来源：http://mib.hfpthk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lmt.yj20258888.top

[Q58] 累计求和
来源：http://edc.yonumen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://leg.cashguo.top

[Q59] 分组内累计
来源：http://she.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wvc.jlsjyb.cn

[Q60] 取上一行 / 下一行
来源：http://kcx.xylfe.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yvh.zhaomingkeji.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mqr.jlsjyb.cn

[Q61] 移动平均
来源：http://pjn.jinyuanbaomall.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cer.chenzaomai.com

[Q62] 分组占比
来源：http://zgx.chenjidiqi.icu

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bzv.mhx1999.top

[Q63] 开启事务
来源：http://myf.zhijiandao.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hej.ydzc1.top

[Q64] 提交事务
来源：http://zeq.ctjpmb.com

COMMIT;
来源：http://raw.xinyue.icu

[Q65] 回滚事务
来源：http://fnw.jqgufenzy.top

ROLLBACK;
来源：http://yfc.uphjek.com

[Q66] 行锁查询
来源：http://bdf.zdbjq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fxu.xinyue.icu

[Q67] 设置隔离级别
来源：http://igh.jqgfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://duh.0kj1m.cn

[Q68] 保存点
来源：http://qlx.jqgfzy.top

SAVEPOINT sp1;
来源：http://did.ppjwa.cn

ROLLBACK TO sp1;
来源：http://yqz.yonumen.top

[Q69] 查看执行计划
来源：http://ceo.52xcode.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rfg.ydjk.org.cn

[Q70] 更新统计信息
来源：http://ckn.zhijiandao.cn

ANALYZE TABLE users;
来源：http://iwi.sjlbkw.cn

[Q71] 查看建表语句
来源：http://vow.dashuyun.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://esa.chenlongwang.top

[Q72] 查看索引
来源：http://ctv.aizwys.cn

SHOW INDEX FROM users;
来源：http://nyp.xuanzx.com

[Q73] 查看表状态
来源：http://jkv.vqdsnc.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cwv.chenzaomai.com

[Q74] 强制使用索引
来源：http://qiu.zhijiandao.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mij.nanxinkj.top

[Q75] 日期格式化
来源：http://hsc.jinqigfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ohc.9152youxi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eow.jyoumei.cn

[Q76] 按天统计
来源：http://zkx.xingfuxueyuan.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cna.yonumen.top

[Q77] 时间加减
来源：http://fdy.jinqigufen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vqy.pengpengdd.cyou

[Q78] 当前时间
来源：http://taw.xziqi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ybb.zhixingplan.top

[Q79] 字符串拼接
来源：http://llq.zhoulong.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dgf.chenzaomai.com

[Q80] 字符串截取
来源：http://rbm.sjlbkw.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xyi.yonumen.top

[Q81] 字符串替换
来源：http://jyl.fehbvm.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jwt.yonumen.top

[Q82] 字符长度与字节长度
来源：http://vyw.ctjpmb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qkz.cheryme.top

[Q83] 大小写转换
来源：http://nkc.jlsjyb.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wja.xylfe.cn

[Q84] 去除首尾空格
来源：http://pwy.gzhubu.top

SELECT TRIM(name) FROM users;
来源：http://bpa.jinyuanbaomall.cn

[Q85] 数值取整
来源：http://qpk.fengsongda.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yqk.vqdsnc.cn

[Q86] 读取 JSON 字段
来源：http://kai.nanxuanxn.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://znd.feifeiyinyue.top

[Q87] JSON 字段做条件
来源：http://sjt.shzxlz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gzt.zycfv.cn

[Q88] 行转列（条件聚合）
来源：http://czg.xinyue.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bny.fanxiaobao.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mwy.gzhubu.top

[Q89] 判断表是否存在
来源：http://vox.tianlin.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vxl.gotoacloud.top

[Q90] 生成序号列
来源：http://pcd.hcnkem.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qvr.zhijiandao.cn

================================================================================
来源：http://wmd.chenjidiqi.icu

R. Bash 专题
来源：http://zfi.jinyuanbaomall.cn

================================================================================
来源：http://rxx.snrcjt.cn

[R01] shebang 与严格模式
来源：http://gxp.316326.xyz

#!/usr/bin/env bash
来源：http://xis.jinqigufen.top

set -euo pipefail
来源：http://hge.gzhubu.top

[R02] 变量赋值与使用
来源：http://urs.fehbvm.com

name="Tom"; echo "$name"
来源：http://rrs.hnxiangtu.top

[R03] 只读变量
来源：http://tai.zhijiandao.cn

readonly PI=3.14
来源：http://scs.hammf.cn

[R04] 位置参数
来源：http://opx.yuanzhike.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ogd.sxryk.cn

[R05] 参数默认值
来源：http://qex.sufxvd.cn

name="${1:-default}"
来源：http://qqo.c1oappe.top

[R06] 判断命令是否存在
来源：http://frc.hcnkem.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iyp.kuanghao11.cn

[R07] if 判断文件
来源：http://qgt.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eva.hesvh.cn

[R08] 数值比较
来源：http://vxl.andypj.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://zsl.zdqjudy.top

[R09] 字符串比较
来源：http://yxp.xinyue.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nzq.yangfankeji.com

[R10] 正则匹配
来源：http://rrf.fengsongda.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ofm.316326.xyz

[R11] case 多分支
来源：http://dri.sysykeji.top

case "$1" in
来源：http://cre.cqqwz.cn

start) echo "启动" ;;
来源：http://tdn.jqgfzy.top

stop)  echo "停止" ;;
来源：http://ayq.cqqwz.cn

*)     echo "未知命令" ;;
来源：http://awt.guowangkeji.top

esac
来源：http://vmg.dianchejie.cn

[R12] for 遍历文件
来源：http://fds.fktsv.cn

for f in *.txt; do echo "$f"; done
来源：http://axp.birdmap.top

[R13] for 计数循环
来源：http://bsb.xylfe.cn

for i in {1..10}; do echo "$i"; done
来源：http://wwo.havefunace.top

[R14] C 风格 for
来源：http://byi.hongshengwenyu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vmq.shzxlz.cn

[R15] while 逐行读文件
来源：http://cmr.hammf.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ywi.jyoumei.cn

[R16] until 等待条件
来源：http://tci.snrcjt.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iev.jinghuilouyu.cn

[R17] 数组定义与取值
来源：http://vso.jiagoushi.top

arr=(a b c); echo "${arr[0]}"
来源：http://dkd.tanke756.top

[R18] 遍历数组
来源：http://gak.meibo888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vkq.gogol.net.cn

[R19] 数组长度
来源：http://hjs.ppjwa.cn

echo "${#arr[@]}"
来源：http://wmr.hnxiangtu.top

[R20] 关联数组（字典）
来源：http://nwi.tianlin.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lkj.jyoumei.cn

[R21] 字符串长度
来源：http://nkf.zdbjq.cn

echo "${#s}"
来源：http://vkd.svipenyu.cn

[R22] 截取子串
来源：http://wdp.sjlbkw.cn

echo "${s:0:5}"
来源：http://wfh.9152youxi.cn

[R23] 字符串替换
来源：http://gth.daxiang520.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xwr.havefunace.top

[R24] 大小写转换
来源：http://hxa.zhijiandao.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rnf.316326.xyz

[R25] 去后缀 / 去前缀
来源：http://dot.zhijiandao.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://imy.vehdjk.com

[R26] 命令替换
来源：http://gmr.chenlongwang.top

now=$(date +%F); echo "$now"
来源：http://igh.tian-w.cn

[R27] 算术展开
来源：http://dsd.birdmap.top

echo $((1 + 2 * 3))
来源：http://nqp.hammf.cn

[R28] 浮点运算
来源：http://kbm.gotoacloud.top

echo "scale=2; 10/3" | bc
来源：http://xyb.xziqi.cn

[R29] 定义函数
来源：http://dyg.dashuyun.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dfk.haohaochexian.top

[R30] 函数返回状态码
来源：http://muv.316326.xyz

f() { return 0; }; f || echo "失败了"
来源：http://wek.iojbl.cn

[R31] 局部变量
来源：http://zkj.shzxlz.cn

f() { local x=1; echo "$x"; }
来源：http://hwp.ybcxt.top

[R32] 参数个数校验
来源：http://xyt.dianchejie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tau.yj20258888.top

[R33] 捕获错误并提示行号
来源：http://mhg.zhijiandao.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rab.meibo888.top

[R34] 退出时清理
来源：http://qto.guowangkeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://fuu.bjfxy.top

[R35] 后台执行并等待
来源：http://eds.ywan-chungtsiang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hnh.xuanzx.com

[R36] 并发执行多个任务
来源：http://ost.yj20258888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://udj.fehbvm.com

[R37] 把输出赋给变量
来源：http://cgf.sjlbkw.cn

files=$(ls -1)
来源：http://ohv.dashuyun.cn

[R38] 管道串联
来源：http://kna.wangdashe.top

cat a.txt | grep -i error | wc -l
来源：http://obt.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://kho.vehdjk.com

cmd > out.log 2>&1
来源：http://arb.shangyingyoupin.top

[R40] 追加写日志
来源：http://uol.zhongyouzk.top

echo "log" >> out.log
来源：http://wke.zhaomingkeji.xyz

[R41] 丢弃输出
来源：http://btj.xziqi.cn

cmd >/dev/null 2>&1
来源：http://ngf.redwolf501.top

[R42] 输入重定向
来源：http://jvj.ctjpmb.com

wc -l < a.txt
来源：http://dsv.jianghu66.top

[R43] 按名字查找文件
来源：http://ryg.c1oappe.top

find . -name "*.log" -type f
来源：http://hxy.shanyushiyangtech.top

[R44] 按修改时间查找
来源：http://rcs.haohaochexian.top

find . -mtime -7 -type f
来源：http://lkf.yfazqb.com

[R45] 批量删除
来源：http://mtr.andypj.xyz

find . -name "*.tmp" -delete
来源：http://zkz.cucudq.cn

[R46] 递归替换文件内容
来源：http://qst.birdmap.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gwd.jiagoushi.top

[R47] sed 单行替换
来源：http://uud.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://nbg.gotoacloud.top

[R48] awk 取指定列
来源：http://mbb.ivvv.top

awk '{print $1, $3}' a.txt
来源：http://gra.dianchejie.cn

[R49] awk 带条件
来源：http://fnd.yj202588.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mru.yj20258.top

[R50] awk 求和
来源：http://lgx.yonumen.top

awk '{s += $2} END {print s}' a.txt
来源：http://bcu.ppjwa.cn

[R51] 排序去重取前几
来源：http://ruu.sysykeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://uvi.jinqigfzy.top

[R52] 统计行数
来源：http://cxx.quarkkingdee.top

wc -l a.txt
来源：http://kkp.shuidangran.top

[R53] 查看文件头与实时尾
来源：http://spj.cashguo.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zix.hongshengwenyu.top

[R54] 比较两个文件
来源：http://oir.shzxlz.cn

diff a.txt b.txt
来源：http://dwv.zhaomingkeji.xyz

[R55] 压缩与解压
来源：http://aty.xziqi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://has.tianlin.xyz

[R56] 远程拷贝
来源：http://vye.uphjek.com

scp file user@host:/path/
来源：http://rtn.uphjek.com

[R57] 远程执行命令
来源：http://uie.dashuyun.cn

ssh user@host 'uptime'
来源：http://iwp.yuxming.cn

[R58] 下载文件
来源：http://fnk.yj20258888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pdl.aibaodan.cn

[R59] 发 POST JSON
来源：http://arh.zhengqikj.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://efr.zhixingplan.top

[R60] 只看 HTTP 状态码
来源：http://alq.sysykeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bzf.vehdjk.com

[R61] 磁盘占用
来源：http://elx.haohaochexian.top

df -h;  du -sh *
来源：http://ipw.c1oappe.top

[R62] 找最占空间的文件
来源：http://ftw.havefunace.top

du -ah . | sort -rh | head -10
来源：http://dnu.c1oappe.top

[R63] 内存与进程
来源：http://uxi.ywan-chungtsiang.top

free -h;  ps aux | grep nginx
来源：http://kou.andypj.xyz

[R64] 结束进程
来源：http://wvd.fzhhl.top

kill -9 $(pgrep -f app.py)
来源：http://kuz.redwolf501.top

[R65] 查看端口占用
来源：http://xuc.chenzaomai.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pho.52xcode.cn

[R66] 定时任务
来源：http://juv.fktsv.cn

crontab -e;  crontab -l
来源：http://qjk.hnxiangtu.top

[R67] 生成随机十六进制串
来源：http://lkq.zdqjudy.top

openssl rand -hex 16
来源：http://ary.yfazqb.com

[R68] 计算文件校验值
来源：http://nrd.daria6918.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ean.zycfv.cn

[R69] 生成随机密码
来源：http://zpt.pengpengdd.cyou

head -c 16 /dev/urandom | base64
来源：http://lxw.wangshuangyany.cn

[R70] 时间戳与互转
来源：http://gkc.ydzc1.top

date +%s;  date -d @1700000000
来源：http://tcl.hesvh.cn

[R71] 日期格式化
来源：http://jpn.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ibm.jinqigufen.top

[R72] 等待端口就绪
来源：http://lhq.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ltn.52xcode.cn

[R73] 分割大日志
来源：http://duv.gotoacloud.top


<!-- 参考信息 -->