代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mky.cashguo.top

[Q24] 去重
来源：http://lyn.tarul.cn

SELECT DISTINCT city FROM users;
来源：http://uom.xuanzx.com

[Q25] 只取前 N 条
来源：http://vxz.zhoulong.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hce.yvedp.cn

[Q26] 计数
来源：http://ptf.chenjidiqi.icu

SELECT COUNT(*) FROM users;
来源：http://xty.jinqigufen.top

[Q27] 条件计数
来源：http://mlp.zhiwuduotai.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mbv.zhixingplan.top

[Q28] 求和与平均
来源：http://mfi.shuidangran.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lro.jiagoushi.top

[Q29] 最大最小值
来源：http://jjs.ybcxt.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://iei.fanxiaobao.xyz

[Q30] 分组统计
来源：http://twm.yongpay.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jrh.zhoulong.xyz

[Q31] 分组后过滤
来源：http://auk.c1oappe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uri.guannengcc.top

[Q32] 分组拼接字符串
来源：http://cea.svipenyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gkk.hnqzz.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ipy.bjfxy.top

[Q33] 多列分组
来源：http://ygs.mhx1999.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rnm.gzhubu.top

[Q34] 每组取第一条
来源：http://dbp.xuanzx.com

SELECT * FROM (
来源：http://fac.nanxinkj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://epp.shzxlz.cn

) t WHERE rn = 1;
来源：http://kgz.jqgfzy.top

[Q35] 内连接
来源：http://dgz.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cmz.vehdjk.com

[Q36] 左连接
来源：http://ncy.316326.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xeo.chenzaomai.com

[Q37] 右连接
来源：http://efb.hywenlv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ntb.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jxv.svipenyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ojc.yanxiufei.cn

[Q39] 自连接（查上下级）
来源：http://lcb.fehbvm.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://bls.yangfankeji.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rpl.vqdsnc.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dxe.ybcxt.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fur.gaohongyu789.top

[Q41] 多表连接
来源：http://xyn.ehwqpu.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://kms.ywan-chungtsiang.top

JOIN users u ON u.id = o.user_id
来源：http://uws.ydjk.org.cn

JOIN products p ON p.id = o.product_id;
来源：http://txt.ydzc1.top

[Q42] 连接条件附加过滤
来源：http://kvt.hammf.cn

SELECT u.name, o.amount FROM users u
来源：http://bos.feifeiyinyue.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dyc.tarul.cn

[Q43] 标量子查询
来源：http://fqw.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fwi.snrcjt.cn

[Q44] IN 子查询
来源：http://bzs.sweek.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://row.zhongyouzk.top

[Q45] EXISTS 判断存在
来源：http://ntc.gaohongyu789.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zgh.c1oappe.top

[Q46] NOT EXISTS 判断不存在
来源：http://zcy.mhx1999.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tzz.zhengqikj.top

[Q47] 与平均值比较
来源：http://hnm.aizwys.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dtm.bjfxy.top

[Q48] CTE 公用表表达式
来源：http://koc.cheryme.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://shb.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://vdt.chenlongwang.top

[Q49] 更新单行
来源：http://fzv.ydzc1.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sil.chenlongwang.top

[Q50] 批量更新
来源：http://qvb.zhoulong.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://txj.nanxinkj.top

[Q51] 用子查询更新
来源：http://ywk.yuxming.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fhr.smart0.xyz

[Q52] 删除指定行
来源：http://vqu.ydzc1.top

DELETE FROM users WHERE id = 10;
来源：http://tny.zhengqikj.top

[Q53] 按条件删除
来源：http://csh.yanxiufei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nve.aizwys.cn

[Q54] 清空表
来源：http://wgl.tanke756.top

TRUNCATE TABLE logs;
来源：http://npy.hnxiangtu.top

[Q55] 排名（并列占位）
来源：http://tgt.9152youxi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pwp.fengsongda.top

[Q56] 密集排名（并列不占位）
来源：http://gjd.yuanzhike.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rjz.fehbvm.com

[Q57] 行号
来源：http://gee.zycfv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wom.zhaomingkeji.xyz

[Q58] 累计求和
来源：http://zla.hcnkem.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zya.yvedp.cn

[Q59] 分组内累计
来源：http://cnv.jinghuilouyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rvs.zhijiandao.cn

[Q60] 取上一行 / 下一行
来源：http://vez.jinghuilouyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://egu.shanyushiyangtech.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://itq.aizwys.cn

[Q61] 移动平均
来源：http://sfi.xuanzx.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xnx.hywenlv.cn

[Q62] 分组占比
来源：http://njc.yuanzhike.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jel.aizwys.cn

[Q63] 开启事务
来源：http://olv.fengsongda.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ipx.redwolf501.top

[Q64] 提交事务
来源：http://xkx.yueranfly.top

COMMIT;
来源：http://xjo.ctjpmb.com

[Q65] 回滚事务
来源：http://qqf.jyoumei.cn

ROLLBACK;
来源：http://tox.ydzc1.top

[Q66] 行锁查询
来源：http://hcd.andypj.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qsb.sweek.top

[Q67] 设置隔离级别
来源：http://gre.cucudq.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zxx.shangyingyoupin.top

[Q68] 保存点
来源：http://asn.nanxinkj.top

SAVEPOINT sp1;
来源：http://tyj.ctjpmb.com

ROLLBACK TO sp1;
来源：http://czh.xinyue.icu

[Q69] 查看执行计划
来源：http://bie.xuetiantiany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mvi.zhixingplan.top

[Q70] 更新统计信息
来源：http://qdl.316326.xyz

ANALYZE TABLE users;
来源：http://eqx.wangdashe.top

[Q71] 查看建表语句
来源：http://qvm.316326.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eva.zhongyouzk.top

[Q72] 查看索引
来源：http://zdo.sysykeji.top

SHOW INDEX FROM users;
来源：http://ydz.hfpthk.cn

[Q73] 查看表状态
来源：http://ndf.aizwys.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zue.daxiang520.top

[Q74] 强制使用索引
来源：http://tqw.sweek.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://iks.snrcjt.cn

[Q75] 日期格式化
来源：http://hwf.sxryk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ymp.iojbl.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vbx.zhaomingkeji.xyz

[Q76] 按天统计
来源：http://imc.0kj1m.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zko.daria6918.cn

[Q77] 时间加减
来源：http://nxp.ppjwa.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://aom.daxiang520.top

[Q78] 当前时间
来源：http://aqq.zhiwuduotai.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bag.sufxvd.cn

[Q79] 字符串拼接
来源：http://tfr.xinyue.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dyf.vqdsnc.cn

[Q80] 字符串截取
来源：http://avo.jianghu66.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ceh.zhoulong.xyz

[Q81] 字符串替换
来源：http://btu.andypj.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qyw.tanke756.top

[Q82] 字符长度与字节长度
来源：http://aep.hnxiangtu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pyw.mhx1999.top

[Q83] 大小写转换
来源：http://mmx.andypj.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fqw.jyoumei.cn

[Q84] 去除首尾空格
来源：http://vms.fengsongda.top

SELECT TRIM(name) FROM users;
来源：http://dyz.zdbjq.cn

[Q85] 数值取整
来源：http://oap.chenjidiqi.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dfi.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://txu.aibaodan.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dif.dashuyun.cn

[Q87] JSON 字段做条件
来源：http://eqb.andypj.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lhz.gogol.net.cn

[Q88] 行转列（条件聚合）
来源：http://ubm.shangyingyoupin.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xbv.zhaomingkeji.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fnw.cdnleiting.top

[Q89] 判断表是否存在
来源：http://mzq.birdmap.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nov.jianghu66.top

[Q90] 生成序号列
来源：http://sra.yuxming.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lnx.guowangkeji.top

================================================================================
来源：http://aax.zycfv.cn

R. Bash 专题
来源：http://fzu.yueranfly.top

================================================================================
来源：http://ghw.kuanghao11.cn

[R01] shebang 与严格模式
来源：http://qaq.yueranfly.top

#!/usr/bin/env bash
来源：http://qob.316326.xyz

set -euo pipefail
来源：http://xnh.xylfe.cn

[R02] 变量赋值与使用
来源：http://ait.haohaochexian.top

name="Tom"; echo "$name"
来源：http://zot.yueranfly.top

[R03] 只读变量
来源：http://ylu.nwbrower.top

readonly PI=3.14
来源：http://lto.cqqwz.cn

[R04] 位置参数
来源：http://jhl.hesvh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fga.uphjek.com

[R05] 参数默认值
来源：http://geo.xuetiantiany.cn

name="${1:-default}"
来源：http://hiq.hfpthk.cn

[R06] 判断命令是否存在
来源：http://dkd.9152youxi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qot.wangdashe.top

[R07] if 判断文件
来源：http://esq.yvedp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://omn.wangdashe.top

[R08] 数值比较
来源：http://cup.jinghuilouyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://isk.uphjek.com

[R09] 字符串比较
来源：http://wfo.meibo888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fxo.sjlbkw.cn

[R10] 正则匹配
来源：http://azf.cqqwz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nos.jqgufenzy.top

[R11] case 多分支
来源：http://jkq.ctjpmb.com

case "$1" in
来源：http://rsk.bbcook.cn

start) echo "启动" ;;
来源：http://hgx.ydjk.org.cn

stop)  echo "停止" ;;
来源：http://xhu.guowangkeji.top

*)     echo "未知命令" ;;
来源：http://zyb.gotoacloud.top

esac
来源：http://wag.ywan-chungtsiang.top

[R12] for 遍历文件
来源：http://aqi.jyoumei.cn

for f in *.txt; do echo "$f"; done
来源：http://ysi.hywenlv.cn

[R13] for 计数循环
来源：http://lej.cheryme.top

for i in {1..10}; do echo "$i"; done
来源：http://lpe.wangdashe.top

[R14] C 风格 for
来源：http://uzf.shanyushiyangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vlk.guowangkeji.top

[R15] while 逐行读文件
来源：http://voc.jiagoushi.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://odv.fzhhl.top

[R16] until 等待条件
来源：http://qlb.jinghuilouyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ijx.yuxming.cn

[R17] 数组定义与取值
来源：http://dij.hnxiangtu.top

arr=(a b c); echo "${arr[0]}"
来源：http://dhn.xuanzx.com

[R18] 遍历数组
来源：http://rlw.ywan-chungtsiang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://axy.hongshengwenyu.top

[R19] 数组长度
来源：http://omb.yfazqb.com

echo "${#arr[@]}"
来源：http://gfj.bjfxy.top

[R20] 关联数组（字典）
来源：http://xpf.shangyingyoupin.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qzw.gogol.net.cn

[R21] 字符串长度
来源：http://dkd.tian-w.cn

echo "${#s}"
来源：http://qsp.jqgufenzy.top

[R22] 截取子串
来源：http://gvt.jinyuanbaomall.cn

echo "${s:0:5}"
来源：http://gdl.chenlongwang.top

[R23] 字符串替换
来源：http://xeq.jianghu66.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tky.yfazqb.com

[R24] 大小写转换
来源：http://ock.xingfuxueyuan.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://srf.0kj1m.cn

[R25] 去后缀 / 去前缀
来源：http://xsv.52xcode.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zwi.cdnleiting.top

[R26] 命令替换
来源：http://gci.iojbl.cn

now=$(date +%F); echo "$now"
来源：http://sib.hnxiangtu.top

[R27] 算术展开
来源：http://idf.zhiwuduotai.top

echo $((1 + 2 * 3))
来源：http://ggm.tianlin.xyz

[R28] 浮点运算
来源：http://nmz.cucudq.cn

echo "scale=2; 10/3" | bc
来源：http://txi.yvedp.cn

[R29] 定义函数
来源：http://fjb.jinyuanbaomall.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ety.iojbl.cn

[R30] 函数返回状态码
来源：http://cos.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://ple.ivvv.top

[R31] 局部变量
来源：http://xzr.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://obg.snrcjt.cn

[R32] 参数个数校验
来源：http://mif.daxiang520.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pth.svipenyu.cn

[R33] 捕获错误并提示行号
来源：http://cyq.xinyue.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ogm.zhixingplan.top

[R34] 退出时清理
来源：http://kql.jinyuanbaomall.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xej.316326.xyz

[R35] 后台执行并等待
来源：http://jcj.jinqigfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tlr.jqgufenzy.top

[R36] 并发执行多个任务
来源：http://xpu.bjfxy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://djq.tarul.cn

[R37] 把输出赋给变量
来源：http://nlm.xinyue.icu

files=$(ls -1)
来源：http://hnu.yj202588.top

[R38] 管道串联
来源：http://mpq.zycfv.cn

cat a.txt | grep -i error | wc -l
来源：http://ryw.zdqjudy.top

[R39] 重定向标准输出与错误
来源：http://wtb.jiagoushi.top

cmd > out.log 2>&1
来源：http://mfw.hcnkem.com

[R40] 追加写日志
来源：http://oup.sweek.top

echo "log" >> out.log
来源：http://lni.zhaomingkeji.xyz

[R41] 丢弃输出
来源：http://qsw.yuxming.cn

cmd >/dev/null 2>&1
来源：http://ewg.zhiwuduotai.top

[R42] 输入重定向
来源：http://xbi.chenzaomai.com

wc -l < a.txt
来源：http://bcn.chenzaomai.com

[R43] 按名字查找文件
来源：http://zie.zhijiandao.cn

find . -name "*.log" -type f
来源：http://lql.fehbvm.com

[R44] 按修改时间查找
来源：http://hro.zhongyouzk.top

find . -mtime -7 -type f
来源：http://qtk.tian-w.cn

[R45] 批量删除
来源：http://oiy.yj20258.top

find . -name "*.tmp" -delete
来源：http://psg.yfazqb.com

[R46] 递归替换文件内容
来源：http://hww.c1oappe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vyt.yj20258888.top

[R47] sed 单行替换
来源：http://tyy.daria6918.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pwc.c1oappe.top

[R48] awk 取指定列
来源：http://nha.bbcook.cn

awk '{print $1, $3}' a.txt
来源：http://osm.pycfn.com

[R49] awk 带条件
来源：http://guv.ctjpmb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://roq.sysykeji.top

[R50] awk 求和
来源：http://ikj.hcnkem.com

awk '{s += $2} END {print s}' a.txt
来源：http://vkv.redwolf501.top

[R51] 排序去重取前几
来源：http://gqf.zhongyouzk.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lzq.vehdjk.com

[R52] 统计行数
来源：http://oll.gaohongyu789.top

wc -l a.txt
来源：http://wdp.xuanzx.com

[R53] 查看文件头与实时尾
来源：http://bsd.zhoulong.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uds.bjfxy.top

[R54] 比较两个文件
来源：http://wcb.zdqjudy.top

diff a.txt b.txt
来源：http://obi.birdmap.top

[R55] 压缩与解压
来源：http://thh.xuetiantiany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ega.nanxinkj.top

[R56] 远程拷贝
来源：http://ces.fanxiaobao.xyz

scp file user@host:/path/
来源：http://etz.shuidangran.top

[R57] 远程执行命令
来源：http://dis.chenlongwang.top

ssh user@host 'uptime'
来源：http://nda.zhengqikj.top

[R58] 下载文件
来源：http://jgf.zhijiandao.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://quc.fktsv.cn

[R59] 发 POST JSON
来源：http://fdf.tianlin.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mrw.hammf.cn

[R60] 只看 HTTP 状态码
来源：http://uzp.gogol.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ojf.snrcjt.cn

[R61] 磁盘占用
来源：http://ljc.nanxuanxn.top

df -h;  du -sh *
来源：http://yuy.jiagoushi.top

[R62] 找最占空间的文件
来源：http://jkf.xuetiantiany.cn

du -ah . | sort -rh | head -10
来源：http://wqd.hnqzz.top

[R63] 内存与进程
来源：http://vna.uphjek.com

free -h;  ps aux | grep nginx
来源：http://ogt.ivvv.top

[R64] 结束进程
来源：http://nqd.birdmap.top

kill -9 $(pgrep -f app.py)
来源：http://rxw.hnxiangtu.top

[R65] 查看端口占用
来源：http://lfm.cheryme.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tbl.zhoulong.xyz

[R66] 定时任务
来源：http://qaj.kuanghao11.cn

crontab -e;  crontab -l
来源：http://nlp.smart0.xyz

[R67] 生成随机十六进制串
来源：http://cid.xziqi.cn

openssl rand -hex 16
来源：http://zhg.jlsjyb.cn

[R68] 计算文件校验值
来源：http://dpa.daxiang520.top

sha256sum a.txt;  md5sum a.txt
来源：http://kwn.shangyingyoupin.top

[R69] 生成随机密码
来源：http://xbo.hesvh.cn

head -c 16 /dev/urandom | base64
来源：http://cbk.jinqigufen.top

[R70] 时间戳与互转
来源：http://isk.jianghu66.top

date +%s;  date -d @1700000000
来源：http://xgf.xuetiantiany.cn

[R71] 日期格式化
来源：http://hff.c1oappe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://gia.yj20258.top

[R72] 等待端口就绪
来源：http://pbi.jinyuanbaomall.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://iis.hesvh.cn

[R73] 分割大日志
来源：http://szp.andypj.xyz


<!-- 参考信息 -->