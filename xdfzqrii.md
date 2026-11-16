代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rhf.chenzaomai.com

[Q24] 去重
来源：http://obu.shanyushiyangkeji.top

SELECT DISTINCT city FROM users;
来源：http://sco.sjlbkw.cn

[Q25] 只取前 N 条
来源：http://ymu.gzhubu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://spk.cashguo.top

[Q26] 计数
来源：http://ijy.ydzc1.top

SELECT COUNT(*) FROM users;
来源：http://qrh.xuanzx.com

[Q27] 条件计数
来源：http://ggy.pycfn.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://onq.fanxiaobao.xyz

[Q28] 求和与平均
来源：http://uwq.zhijiandao.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fnz.ivvv.top

[Q29] 最大最小值
来源：http://vht.ctjpmb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://sio.vqdsnc.cn

[Q30] 分组统计
来源：http://rax.0kj1m.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jif.jyoumei.cn

[Q31] 分组后过滤
来源：http://gze.xuanzx.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yds.sxryk.cn

[Q32] 分组拼接字符串
来源：http://rft.fzhhl.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tcl.cqqwz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://frg.ywan-chungtsiang.top

[Q33] 多列分组
来源：http://srm.ydzc1.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://csz.guannengcc.top

[Q34] 每组取第一条
来源：http://knt.gogol.net.cn

SELECT * FROM (
来源：http://cvm.ehwqpu.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uhv.yuanzhike.top

) t WHERE rn = 1;
来源：http://cot.zhoulong.xyz

[Q35] 内连接
来源：http://kkl.jiagoushi.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lcx.zhijiandao.cn

[Q36] 左连接
来源：http://fho.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://muq.sxryk.cn

[Q37] 右连接
来源：http://ndi.quarkkingdee.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eah.hammf.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kfe.andypj.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ina.jinqigfzy.top

[Q39] 自连接（查上下级）
来源：http://hyp.wangshuangyany.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lkg.pengpengdd.cyou

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://las.fzhhl.top

[Q40] 交叉连接（笛卡尔积）
来源：http://typ.pengpengdd.cyou

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oca.guowangkeji.top

[Q41] 多表连接
来源：http://mlx.yonumen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cgz.jinghuilouyu.cn

JOIN users u ON u.id = o.user_id
来源：http://nkl.jqgufenzy.top

JOIN products p ON p.id = o.product_id;
来源：http://xrh.shangyingyoupin.top

[Q42] 连接条件附加过滤
来源：http://hxb.ydzc1.top

SELECT u.name, o.amount FROM users u
来源：http://gcz.chenzaomai.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dzz.hnxiangtu.top

[Q43] 标量子查询
来源：http://soq.ywan-chungtsiang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iyc.zhaomingkeji.xyz

[Q44] IN 子查询
来源：http://coq.jqgufenzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ahk.shanyushiyangtech.top

[Q45] EXISTS 判断存在
来源：http://vus.jinyuanbaomall.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ljy.jinqigfzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://xxf.jqgufenzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eoe.shuidangran.top

[Q47] 与平均值比较
来源：http://cvj.316326.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ykd.xuanzx.com

[Q48] CTE 公用表表达式
来源：http://nig.pengpengdd.cyou

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qkl.sxryk.cn

SELECT * FROM t WHERE c > 5;
来源：http://pbr.aibaodan.cn

[Q49] 更新单行
来源：http://fnm.0kj1m.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yed.hfpthk.cn

[Q50] 批量更新
来源：http://arl.xziqi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zly.shanyushiyangkeji.top

[Q51] 用子查询更新
来源：http://pul.ybcxt.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wxp.guowangkeji.top

[Q52] 删除指定行
来源：http://txt.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://msr.sxryk.cn

[Q53] 按条件删除
来源：http://rgs.svipenyu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ifj.fanxiaobao.xyz

[Q54] 清空表
来源：http://hjt.jinghuilouyu.cn

TRUNCATE TABLE logs;
来源：http://zbq.hcnkem.com

[Q55] 排名（并列占位）
来源：http://hre.sjlbkw.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tbg.zhaomingkeji.xyz

[Q56] 密集排名（并列不占位）
来源：http://xza.jianghu66.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tyg.cheryme.top

[Q57] 行号
来源：http://gka.hcnkem.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hha.yvedp.cn

[Q58] 累计求和
来源：http://iyp.yueranfly.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nvh.jyoumei.cn

[Q59] 分组内累计
来源：http://nfq.jiagoushi.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ptk.yj202588.top

[Q60] 取上一行 / 下一行
来源：http://dgf.jinqigfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wzf.xinyue.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dcc.xylfe.cn

[Q61] 移动平均
来源：http://grz.chenzaomai.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qhh.zycfv.cn

[Q62] 分组占比
来源：http://awg.daxiang520.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://avv.ybcxt.top

[Q63] 开启事务
来源：http://ngu.shuidangran.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tdb.sufxvd.cn

[Q64] 提交事务
来源：http://ivr.0kj1m.cn

COMMIT;
来源：http://hyw.wangshuangyany.cn

[Q65] 回滚事务
来源：http://ess.ivvv.top

ROLLBACK;
来源：http://gpd.tarul.cn

[Q66] 行锁查询
来源：http://red.aibaodan.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://khi.hywenlv.cn

[Q67] 设置隔离级别
来源：http://nim.havefunace.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://drr.pycfn.com

[Q68] 保存点
来源：http://cyn.jiagoushi.top

SAVEPOINT sp1;
来源：http://adh.yuxming.cn

ROLLBACK TO sp1;
来源：http://ore.meibo888.top

[Q69] 查看执行计划
来源：http://zoz.sxryk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jci.xuanzx.com

[Q70] 更新统计信息
来源：http://zya.ybcxt.top

ANALYZE TABLE users;
来源：http://gqv.snrcjt.cn

[Q71] 查看建表语句
来源：http://muo.dashuyun.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xiv.zhengqikj.top

[Q72] 查看索引
来源：http://qfi.shanyushiyangtech.top

SHOW INDEX FROM users;
来源：http://suz.hysaishi.cn

[Q73] 查看表状态
来源：http://nzd.jinyuanbaomall.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://src.havefunace.top

[Q74] 强制使用索引
来源：http://zro.cdnleiting.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ube.uphjek.com

[Q75] 日期格式化
来源：http://quv.xuetiantiany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ndq.andypj.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gyp.52xcode.cn

[Q76] 按天统计
来源：http://xyv.aizwys.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ttv.bjfxy.top

[Q77] 时间加减
来源：http://uep.xinyue.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ybb.epnwcf.com

[Q78] 当前时间
来源：http://urs.yvedp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wbp.cqqwz.cn

[Q79] 字符串拼接
来源：http://aqp.guannengcc.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pnc.fktsv.cn

[Q80] 字符串截取
来源：http://xts.fengsongda.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://shn.ybcxt.top

[Q81] 字符串替换
来源：http://uve.quarkkingdee.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hmn.mhx1999.top

[Q82] 字符长度与字节长度
来源：http://dki.dianchejie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://foh.xingfuxueyuan.xyz

[Q83] 大小写转换
来源：http://tmv.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://omq.uphjek.com

[Q84] 去除首尾空格
来源：http://bjg.yuanzhike.top

SELECT TRIM(name) FROM users;
来源：http://ese.yanxiufei.cn

[Q85] 数值取整
来源：http://eei.shangyingyoupin.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://smb.shuidangran.top

[Q86] 读取 JSON 字段
来源：http://bex.meibo888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pfq.uphjek.com

[Q87] JSON 字段做条件
来源：http://kad.0kj1m.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://afj.chenzaomai.com

[Q88] 行转列（条件聚合）
来源：http://ghs.ehwqpu.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gtr.zhaomingkeji.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tnz.zhengqikj.top

[Q89] 判断表是否存在
来源：http://vzm.yj202588.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://azo.zhongyouzk.top

[Q90] 生成序号列
来源：http://qoh.cashguo.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kij.c1oappe.top

================================================================================
来源：http://zrf.hfpthk.cn

R. Bash 专题
来源：http://pkd.uphjek.com

================================================================================
来源：http://zvz.iojbl.cn

[R01] shebang 与严格模式
来源：http://mds.pycfn.com

#!/usr/bin/env bash
来源：http://clf.shangyingyoupin.top

set -euo pipefail
来源：http://hua.gogol.net.cn

[R02] 变量赋值与使用
来源：http://tdt.cheryme.top

name="Tom"; echo "$name"
来源：http://box.daxiang520.top

[R03] 只读变量
来源：http://aek.cqqwz.cn

readonly PI=3.14
来源：http://asc.ctjpmb.com

[R04] 位置参数
来源：http://iad.cucudq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://caf.zhijiandao.cn

[R05] 参数默认值
来源：http://zbf.zdbjq.cn

name="${1:-default}"
来源：http://vzy.xylfe.cn

[R06] 判断命令是否存在
来源：http://wtw.gzhubu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zsh.sjlbkw.cn

[R07] if 判断文件
来源：http://qxw.jlsjyb.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lgg.mhx1999.top

[R08] 数值比较
来源：http://ujl.9152youxi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tfi.kuanghao11.cn

[R09] 字符串比较
来源：http://owh.cdnleiting.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://euq.xuanzx.com

[R10] 正则匹配
来源：http://euf.fengsongda.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://erk.smart0.xyz

[R11] case 多分支
来源：http://qml.fehbvm.com

case "$1" in
来源：http://izc.mhx1999.top

start) echo "启动" ;;
来源：http://buu.havefunace.top

stop)  echo "停止" ;;
来源：http://jnk.vehdjk.com

*)     echo "未知命令" ;;
来源：http://jfo.yvedp.cn

esac
来源：http://jtm.zhoulong.xyz

[R12] for 遍历文件
来源：http://dpe.hesvh.cn

for f in *.txt; do echo "$f"; done
来源：http://yxm.zycfv.cn

[R13] for 计数循环
来源：http://hig.ivvv.top

for i in {1..10}; do echo "$i"; done
来源：http://nwu.cdnleiting.top

[R14] C 风格 for
来源：http://spx.zdqjudy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dsv.yuxming.cn

[R15] while 逐行读文件
来源：http://wow.316326.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cgs.zhijiandao.cn

[R16] until 等待条件
来源：http://dde.hnxiangtu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wqf.xingfuxueyuan.xyz

[R17] 数组定义与取值
来源：http://hwh.yvedp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cmk.dianchejie.cn

[R18] 遍历数组
来源：http://jzo.0kj1m.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://czo.jqgfzy.top

[R19] 数组长度
来源：http://bqu.shuidangran.top

echo "${#arr[@]}"
来源：http://tlg.jinqigfzy.top

[R20] 关联数组（字典）
来源：http://toi.wangdashe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qiz.hcnkem.com

[R21] 字符串长度
来源：http://tuj.jyoumei.cn

echo "${#s}"
来源：http://ecz.iojbl.cn

[R22] 截取子串
来源：http://mop.zhiwuduotai.top

echo "${s:0:5}"
来源：http://qyk.uphjek.com

[R23] 字符串替换
来源：http://tap.gotoacloud.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://asj.jinyuanbaomall.cn

[R24] 大小写转换
来源：http://xdk.xziqi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vqd.cashguo.top

[R25] 去后缀 / 去前缀
来源：http://fuh.jyoumei.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uxr.svipenyu.cn

[R26] 命令替换
来源：http://sza.aizwys.cn

now=$(date +%F); echo "$now"
来源：http://tsr.ybcxt.top

[R27] 算术展开
来源：http://bni.haohaochexian.top

echo $((1 + 2 * 3))
来源：http://jlg.ivvv.top

[R28] 浮点运算
来源：http://dys.gzhubu.top

echo "scale=2; 10/3" | bc
来源：http://siw.yj20258888.top

[R29] 定义函数
来源：http://fdl.aibaodan.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://awh.tianlin.xyz

[R30] 函数返回状态码
来源：http://ihm.sweek.top

f() { return 0; }; f || echo "失败了"
来源：http://hxd.ppjwa.cn

[R31] 局部变量
来源：http://jbp.jiagoushi.top

f() { local x=1; echo "$x"; }
来源：http://sui.tanke756.top

[R32] 参数个数校验
来源：http://cep.sweek.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://byr.tarul.cn

[R33] 捕获错误并提示行号
来源：http://cdi.jiagoushi.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yog.uphjek.com

[R34] 退出时清理
来源：http://kfc.pycfn.com

trap 'rm -f "$tmp"' EXIT
来源：http://ths.gotoacloud.top

[R35] 后台执行并等待
来源：http://xre.smart0.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://sut.jinghuilouyu.cn

[R36] 并发执行多个任务
来源：http://zph.jinqigufen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ywl.aibaodan.cn

[R37] 把输出赋给变量
来源：http://jjf.daxiang520.top

files=$(ls -1)
来源：http://sxg.jyoumei.cn

[R38] 管道串联
来源：http://vvg.hnxiangtu.top

cat a.txt | grep -i error | wc -l
来源：http://mgh.sufxvd.cn

[R39] 重定向标准输出与错误
来源：http://llg.snrcjt.cn

cmd > out.log 2>&1
来源：http://jkl.yuxming.cn

[R40] 追加写日志
来源：http://tdc.jlsjyb.cn

echo "log" >> out.log
来源：http://ovy.zhoulong.xyz

[R41] 丢弃输出
来源：http://ztm.guannengcc.top

cmd >/dev/null 2>&1
来源：http://ofl.tian-w.cn

[R42] 输入重定向
来源：http://svm.vqdsnc.cn

wc -l < a.txt
来源：http://sgw.jyoumei.cn

[R43] 按名字查找文件
来源：http://ajm.hnqzz.top

find . -name "*.log" -type f
来源：http://orm.feifeiyinyue.top

[R44] 按修改时间查找
来源：http://hqj.hnxiangtu.top

find . -mtime -7 -type f
来源：http://pxj.cucudq.cn

[R45] 批量删除
来源：http://ntd.jinqigfzy.top

find . -name "*.tmp" -delete
来源：http://ooc.nanxuanxn.top

[R46] 递归替换文件内容
来源：http://qks.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://aor.chenjidiqi.icu

[R47] sed 单行替换
来源：http://smw.vqdsnc.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ehr.52xcode.cn

[R48] awk 取指定列
来源：http://gfu.dashuyun.cn

awk '{print $1, $3}' a.txt
来源：http://mnx.gaohongyu789.top

[R49] awk 带条件
来源：http://rsm.jianghu66.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cno.zhixingplan.top

[R50] awk 求和
来源：http://ioe.hammf.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zyp.hfpthk.cn

[R51] 排序去重取前几
来源：http://ubb.snrcjt.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lva.chenlongwang.top

[R52] 统计行数
来源：http://hme.mhx1999.top

wc -l a.txt
来源：http://abo.havefunace.top

[R53] 查看文件头与实时尾
来源：http://yvl.ydzc1.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://juv.yueranfly.top

[R54] 比较两个文件
来源：http://jjc.jinghuilouyu.cn

diff a.txt b.txt
来源：http://fug.havefunace.top

[R55] 压缩与解压
来源：http://mye.gaohongyu789.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://btt.jyoumei.cn

[R56] 远程拷贝
来源：http://tla.c1oappe.top

scp file user@host:/path/
来源：http://wnd.hysaishi.cn

[R57] 远程执行命令
来源：http://mhr.mhx1999.top

ssh user@host 'uptime'
来源：http://jao.nwbrower.top

[R58] 下载文件
来源：http://jkh.hammf.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jwv.9152youxi.cn

[R59] 发 POST JSON
来源：http://aav.birdmap.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://brg.cashguo.top

[R60] 只看 HTTP 状态码
来源：http://vgc.andypj.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://izw.ydzc1.top

[R61] 磁盘占用
来源：http://idm.xinyue.icu

df -h;  du -sh *
来源：http://kuv.fengsongda.top

[R62] 找最占空间的文件
来源：http://ncm.jqgufenzy.top

du -ah . | sort -rh | head -10
来源：http://phl.gogol.net.cn

[R63] 内存与进程
来源：http://gux.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://wrg.gogol.net.cn

[R64] 结束进程
来源：http://wke.yj20258.top

kill -9 $(pgrep -f app.py)
来源：http://kqc.zdqjudy.top

[R65] 查看端口占用
来源：http://ist.iojbl.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rgf.ywan-chungtsiang.top

[R66] 定时任务
来源：http://qde.meibo888.top

crontab -e;  crontab -l
来源：http://zit.chenlongwang.top

[R67] 生成随机十六进制串
来源：http://hua.dashuyun.cn

openssl rand -hex 16
来源：http://iqv.yj20258.top

[R68] 计算文件校验值
来源：http://ouo.0kj1m.cn

sha256sum a.txt;  md5sum a.txt
来源：http://egy.svipenyu.cn

[R69] 生成随机密码
来源：http://ucv.jqgufenzy.top

head -c 16 /dev/urandom | base64
来源：http://rlq.shangyingyoupin.top

[R70] 时间戳与互转
来源：http://wdl.316326.xyz

date +%s;  date -d @1700000000
来源：http://wal.jiagoushi.top

[R71] 日期格式化
来源：http://anq.ivvv.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bzq.gotoacloud.top

[R72] 等待端口就绪
来源：http://buc.nwbrower.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wrs.chenzaomai.com

[R73] 分割大日志
来源：http://akn.kuanghao11.cn


<!-- 参考信息 -->