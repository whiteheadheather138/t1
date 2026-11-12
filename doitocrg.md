代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://dpl.vqdsnc.cn

[Q30] 分组统计
来源：http://jrn.yongpay.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://odt.zhijiandao.cn

[Q31] 分组后过滤
来源：http://iwx.jqgufenzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wbr.xuetiantiany.cn

[Q32] 分组拼接字符串
来源：http://zwd.feifeiyinyue.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vul.xingfuxueyuan.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dzf.316326.xyz

[Q33] 多列分组
来源：http://koi.yueranfly.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dqy.gaohongyu789.top

[Q34] 每组取第一条
来源：http://vif.bjfxy.top

SELECT * FROM (
来源：http://fnp.wangshuangyany.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ltb.uphjek.com

) t WHERE rn = 1;
来源：http://dlg.tian-w.cn

[Q35] 内连接
来源：http://vqs.gogol.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qre.haohaochexian.top

[Q36] 左连接
来源：http://llf.fengsongda.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yqx.nwbrower.top

[Q37] 右连接
来源：http://tox.jiagoushi.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qsm.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rxo.ehwqpu.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://byg.tian-w.cn

[Q39] 自连接（查上下级）
来源：http://oqz.ydzc1.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jrt.fktsv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cyt.iojbl.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sae.zdbjq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zrr.zhaomingkeji.xyz

[Q41] 多表连接
来源：http://vrt.ctjpmb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://yaa.yfazqb.com

JOIN users u ON u.id = o.user_id
来源：http://nsm.ydjk.org.cn

JOIN products p ON p.id = o.product_id;
来源：http://jky.ehwqpu.com

[Q42] 连接条件附加过滤
来源：http://bxr.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u
来源：http://ydo.0kj1m.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lgs.havefunace.top

[Q43] 标量子查询
来源：http://zmr.hnxiangtu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://euj.redwolf501.top

[Q44] IN 子查询
来源：http://aan.sjlbkw.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://luz.xinyue.icu

[Q45] EXISTS 判断存在
来源：http://mxg.nwbrower.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lwd.tarul.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ajm.jiagoushi.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mok.havefunace.top

[Q47] 与平均值比较
来源：http://aes.hnqzz.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hea.ctjpmb.com

[Q48] CTE 公用表表达式
来源：http://kln.yj202588.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qkg.hongshengwenyu.top

SELECT * FROM t WHERE c > 5;
来源：http://fek.jinqigfzy.top

[Q49] 更新单行
来源：http://cjj.sjlbkw.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oqv.gogol.net.cn

[Q50] 批量更新
来源：http://twl.yuxming.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hdz.aizwys.cn

[Q51] 用子查询更新
来源：http://bgb.yanxiufei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dsf.hnqzz.top

[Q52] 删除指定行
来源：http://tnr.hammf.cn

DELETE FROM users WHERE id = 10;
来源：http://gca.andypj.xyz

[Q53] 按条件删除
来源：http://ofc.mhx1999.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hrv.nanxinkj.top

[Q54] 清空表
来源：http://aqe.zdqjudy.top

TRUNCATE TABLE logs;
来源：http://qtn.chenlongwang.top

[Q55] 排名（并列占位）
来源：http://ihy.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fzh.sxryk.cn

[Q56] 密集排名（并列不占位）
来源：http://gyq.nwbrower.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xeq.cheryme.top

[Q57] 行号
来源：http://sgc.havefunace.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://srk.xingfuxueyuan.xyz

[Q58] 累计求和
来源：http://xov.nanxinkj.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dxl.chenjidiqi.icu

[Q59] 分组内累计
来源：http://tdh.cheryme.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://toc.zdbjq.cn

[Q60] 取上一行 / 下一行
来源：http://zpd.yuanzhike.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vjz.fzhhl.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qqx.316326.xyz

[Q61] 移动平均
来源：http://cgo.gaohongyu789.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ijo.ybcxt.top

[Q62] 分组占比
来源：http://wed.havefunace.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bby.nwbrower.top

[Q63] 开启事务
来源：http://eeo.kuanghao11.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vwc.fktsv.cn

[Q64] 提交事务
来源：http://bwz.shuidangran.top

COMMIT;
来源：http://afy.yanxiufei.cn

[Q65] 回滚事务
来源：http://qub.shuidangran.top

ROLLBACK;
来源：http://rit.tian-w.cn

[Q66] 行锁查询
来源：http://ywr.shzxlz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://brx.ydjk.org.cn

[Q67] 设置隔离级别
来源：http://bwh.bbcook.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zzr.andypj.xyz

[Q68] 保存点
来源：http://lfj.zhongyouzk.top

SAVEPOINT sp1;
来源：http://wsv.ybcxt.top

ROLLBACK TO sp1;
来源：http://nuj.zhongyouzk.top

[Q69] 查看执行计划
来源：http://jvo.guowangkeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mwn.316326.xyz

[Q70] 更新统计信息
来源：http://lnp.andypj.xyz

ANALYZE TABLE users;
来源：http://xip.nwbrower.top

[Q71] 查看建表语句
来源：http://nol.vqdsnc.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ixk.bbcook.cn

[Q72] 查看索引
来源：http://fug.ehwqpu.com

SHOW INDEX FROM users;
来源：http://zsq.yangfankeji.com

[Q73] 查看表状态
来源：http://vam.sjlbkw.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zpp.chenzaomai.com

[Q74] 强制使用索引
来源：http://hhe.yueranfly.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jii.jqgufenzy.top

[Q75] 日期格式化
来源：http://fhp.hywenlv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sek.jianghu66.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uml.nanxinkj.top

[Q76] 按天统计
来源：http://ode.tarul.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oka.kuanghao11.cn

[Q77] 时间加减
来源：http://xib.shanyushiyangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uwq.xuetiantiany.cn

[Q78] 当前时间
来源：http://cyr.zhoulong.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rpm.yuxming.cn

[Q79] 字符串拼接
来源：http://wyt.tian-w.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://php.xingfuxueyuan.xyz

[Q80] 字符串截取
来源：http://uyt.ivvv.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://btb.xinyue.icu

[Q81] 字符串替换
来源：http://ghm.chenzaomai.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fmi.daxiang520.top

[Q82] 字符长度与字节长度
来源：http://ber.yj20258888.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qdp.jinghuilouyu.cn

[Q83] 大小写转换
来源：http://fyh.xylfe.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fkb.xuetiantiany.cn

[Q84] 去除首尾空格
来源：http://ylv.sysykeji.top

SELECT TRIM(name) FROM users;
来源：http://grq.nanxuanxn.top

[Q85] 数值取整
来源：http://fbf.fengsongda.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vju.zhixingplan.top

[Q86] 读取 JSON 字段
来源：http://jhe.sxryk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cxs.iojbl.cn

[Q87] JSON 字段做条件
来源：http://mvq.cashguo.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nfk.c1oappe.top

[Q88] 行转列（条件聚合）
来源：http://hxn.wangshuangyany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qaq.jinyuanbaomall.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://glh.ppjwa.cn

[Q89] 判断表是否存在
来源：http://xsc.xingfuxueyuan.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://avu.guowangkeji.top

[Q90] 生成序号列
来源：http://mpa.shangyingyoupin.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ioo.gzhubu.top

================================================================================
来源：http://xvc.wangshuangyany.cn

R. Bash 专题
来源：http://kwf.jyoumei.cn

================================================================================
来源：http://lyh.fktsv.cn

[R01] shebang 与严格模式
来源：http://qgf.zycfv.cn

#!/usr/bin/env bash
来源：http://voc.bbcook.cn

set -euo pipefail
来源：http://yni.yonumen.top

[R02] 变量赋值与使用
来源：http://rmx.quarkkingdee.top

name="Tom"; echo "$name"
来源：http://gjf.gogol.net.cn

[R03] 只读变量
来源：http://beg.ppjwa.cn

readonly PI=3.14
来源：http://zes.cashguo.top

[R04] 位置参数
来源：http://cwi.shangyingyoupin.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rmz.hongshengwenyu.top

[R05] 参数默认值
来源：http://wkw.mhx1999.top

name="${1:-default}"
来源：http://anz.bjfxy.top

[R06] 判断命令是否存在
来源：http://mfw.shanyushiyangtech.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vmz.cashguo.top

[R07] if 判断文件
来源：http://yyd.yuanzhike.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bfx.quarkkingdee.top

[R08] 数值比较
来源：http://ucc.jiagoushi.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dgx.ywan-chungtsiang.top

[R09] 字符串比较
来源：http://aml.hnxiangtu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ffl.xuetiantiany.cn

[R10] 正则匹配
来源：http://zrw.aibaodan.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://djj.yfazqb.com

[R11] case 多分支
来源：http://zkr.quarkkingdee.top

case "$1" in
来源：http://abg.yfazqb.com

start) echo "启动" ;;
来源：http://txn.dashuyun.cn

stop)  echo "停止" ;;
来源：http://stk.ctjpmb.com

*)     echo "未知命令" ;;
来源：http://woc.jiagoushi.top

esac
来源：http://mbv.xuanzx.com

[R12] for 遍历文件
来源：http://tia.jianghu66.top

for f in *.txt; do echo "$f"; done
来源：http://mhk.gotoacloud.top

[R13] for 计数循环
来源：http://ejy.smart0.xyz

for i in {1..10}; do echo "$i"; done
来源：http://kcq.yueranfly.top

[R14] C 风格 for
来源：http://erw.jinqigfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uui.smart0.xyz

[R15] while 逐行读文件
来源：http://vnl.shuidangran.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zmm.hongshengwenyu.top

[R16] until 等待条件
来源：http://wme.pycfn.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nxt.gzhubu.top

[R17] 数组定义与取值
来源：http://pqw.jyoumei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bjt.shzxlz.cn

[R18] 遍历数组
来源：http://usr.zhongyouzk.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://heu.fengsongda.top

[R19] 数组长度
来源：http://lgf.aizwys.cn

echo "${#arr[@]}"
来源：http://vik.316326.xyz

[R20] 关联数组（字典）
来源：http://jic.iojbl.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wwf.ppjwa.cn

[R21] 字符串长度
来源：http://qin.hysaishi.cn

echo "${#s}"
来源：http://wdf.yj202588.top

[R22] 截取子串
来源：http://pdf.jinghuilouyu.cn

echo "${s:0:5}"
来源：http://nyl.xylfe.cn

[R23] 字符串替换
来源：http://pui.havefunace.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vpf.chenjidiqi.icu

[R24] 大小写转换
来源：http://nix.xingfuxueyuan.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://qgm.shanyushiyangtech.top

[R25] 去后缀 / 去前缀
来源：http://cxm.hywenlv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vgu.gogol.net.cn

[R26] 命令替换
来源：http://fcu.yj20258.top

now=$(date +%F); echo "$now"
来源：http://bpi.cqqwz.cn

[R27] 算术展开
来源：http://tls.feifeiyinyue.top

echo $((1 + 2 * 3))
来源：http://nir.jiagoushi.top

[R28] 浮点运算
来源：http://ptg.hysaishi.cn

echo "scale=2; 10/3" | bc
来源：http://ers.xuetiantiany.cn

[R29] 定义函数
来源：http://sts.bbcook.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uht.hnqzz.top

[R30] 函数返回状态码
来源：http://djo.pengpengdd.cyou

f() { return 0; }; f || echo "失败了"
来源：http://llx.cashguo.top

[R31] 局部变量
来源：http://bmu.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://tyz.9152youxi.cn

[R32] 参数个数校验
来源：http://mmu.yj20258888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pdw.epnwcf.com

[R33] 捕获错误并提示行号
来源：http://nkl.tian-w.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fgh.zdbjq.cn

[R34] 退出时清理
来源：http://gka.jinghuilouyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://asf.haohaochexian.top

[R35] 后台执行并等待
来源：http://okc.hywenlv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ikt.nanxuanxn.top

[R36] 并发执行多个任务
来源：http://dwb.jiagoushi.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xdb.svipenyu.cn

[R37] 把输出赋给变量
来源：http://sjg.daria6918.cn

files=$(ls -1)
来源：http://zws.jinyuanbaomall.cn

[R38] 管道串联
来源：http://zqi.hfpthk.cn

cat a.txt | grep -i error | wc -l
来源：http://tnd.feifeiyinyue.top

[R39] 重定向标准输出与错误
来源：http://hbs.cqqwz.cn

cmd > out.log 2>&1
来源：http://wwc.tarul.cn

[R40] 追加写日志
来源：http://opz.zdbjq.cn

echo "log" >> out.log
来源：http://dnd.zhengqikj.top

[R41] 丢弃输出
来源：http://eme.yueranfly.top

cmd >/dev/null 2>&1
来源：http://gxe.xziqi.cn

[R42] 输入重定向
来源：http://jtf.bjfxy.top

wc -l < a.txt
来源：http://oqg.xinyue.icu

[R43] 按名字查找文件
来源：http://lbt.havefunace.top

find . -name "*.log" -type f
来源：http://zbs.hysaishi.cn

[R44] 按修改时间查找
来源：http://mkd.zhixingplan.top

find . -mtime -7 -type f
来源：http://ylc.cheryme.top

[R45] 批量删除
来源：http://ihr.zycfv.cn

find . -name "*.tmp" -delete
来源：http://ilb.mhx1999.top

[R46] 递归替换文件内容
来源：http://jlr.vehdjk.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dra.jinghuilouyu.cn

[R47] sed 单行替换
来源：http://ycs.jinghuilouyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xyq.dianchejie.cn

[R48] awk 取指定列
来源：http://lgp.xziqi.cn

awk '{print $1, $3}' a.txt
来源：http://agn.vehdjk.com

[R49] awk 带条件
来源：http://jfr.daxiang520.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sch.chenjidiqi.icu

[R50] awk 求和
来源：http://gmc.yj20258.top

awk '{s += $2} END {print s}' a.txt
来源：http://dsn.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://bsj.iojbl.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yjs.9152youxi.cn

[R52] 统计行数
来源：http://zqw.yuanzhike.top

wc -l a.txt
来源：http://coa.shzxlz.cn

[R53] 查看文件头与实时尾
来源：http://aho.bjfxy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kwl.hysaishi.cn

[R54] 比较两个文件
来源：http://tes.feifeiyinyue.top

diff a.txt b.txt
来源：http://cbr.shuidangran.top

[R55] 压缩与解压
来源：http://ivb.zhijiandao.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ran.bbcook.cn

[R56] 远程拷贝
来源：http://naj.yfazqb.com

scp file user@host:/path/
来源：http://dow.yonumen.top

[R57] 远程执行命令
来源：http://qxa.chenjidiqi.icu

ssh user@host 'uptime'
来源：http://uxm.chenzaomai.com

[R58] 下载文件
来源：http://unf.jiagoushi.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://umn.wangshuangyany.cn

[R59] 发 POST JSON
来源：http://jjw.hnxiangtu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yai.zhixingplan.top

[R60] 只看 HTTP 状态码
来源：http://bxs.cucudq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ycy.pycfn.com

[R61] 磁盘占用
来源：http://yzr.meibo888.top

df -h;  du -sh *
来源：http://hmc.nanxuanxn.top

[R62] 找最占空间的文件
来源：http://yki.nwbrower.top

du -ah . | sort -rh | head -10
来源：http://yfy.tarul.cn

[R63] 内存与进程
来源：http://bgi.hnxiangtu.top

free -h;  ps aux | grep nginx
来源：http://tlx.fehbvm.com

[R64] 结束进程
来源：http://zpv.zhixingplan.top

kill -9 $(pgrep -f app.py)
来源：http://txb.yj202588.top

[R65] 查看端口占用
来源：http://rig.tarul.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bze.chenjidiqi.icu

[R66] 定时任务
来源：http://cyh.wangdashe.top

crontab -e;  crontab -l
来源：http://iop.yueranfly.top

[R67] 生成随机十六进制串
来源：http://nin.fanxiaobao.xyz

openssl rand -hex 16
来源：http://gat.zhiwuduotai.top

[R68] 计算文件校验值
来源：http://fwd.shangyingyoupin.top

sha256sum a.txt;  md5sum a.txt
来源：http://ngx.gotoacloud.top

[R69] 生成随机密码
来源：http://zvv.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://hgw.ybcxt.top

[R70] 时间戳与互转
来源：http://wyn.xylfe.cn

date +%s;  date -d @1700000000
来源：http://rek.jqgfzy.top

[R71] 日期格式化
来源：http://yvg.zdqjudy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kcf.c1oappe.top

[R72] 等待端口就绪
来源：http://xoq.zhongyouzk.top

until nc -z localhost 3306; do sleep 1; done
来源：http://tsz.chenjidiqi.icu

[R73] 分割大日志
来源：http://ykz.mhx1999.top

split -l 1000 big.log part_
来源：http://iwq.jqgfzy.top

[R74] 批量重命名
来源：http://rlg.xziqi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qlf.redwolf501.top

[R75] 导出环境变量
来源：http://gnx.ctjpmb.com

export PATH="$HOME/bin:$PATH"
来源：http://ovo.wangdashe.top

[R76] 使用临时文件
来源：http://ytx.52xcode.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kan.ydzc1.top

[R77] 读取用户输入
来源：http://qtp.uphjek.com

read -rp "请输入: " ans
来源：http://xxp.xziqi.cn

[R78] 交互式菜单
来源：http://niq.316326.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://obg.nanxinkj.top

[R79] 解析命令行选项
来源：http://mws.jyoumei.cn


<!-- 参考信息 -->