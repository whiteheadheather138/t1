代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://qmk.bbcook.cn

[Q30] 分组统计
来源：http://mhp.nwbrower.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dhr.tarul.cn

[Q31] 分组后过滤
来源：http://pch.zhongyouzk.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xxk.ydjk.org.cn

[Q32] 分组拼接字符串
来源：http://bhv.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vnr.yueranfly.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://twt.jinyuanbaomall.cn

[Q33] 多列分组
来源：http://hqw.tianlin.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nic.fengsongda.top

[Q34] 每组取第一条
来源：http://qdq.52xcode.cn

SELECT * FROM (
来源：http://sjy.ehwqpu.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pid.xuanzx.com

) t WHERE rn = 1;
来源：http://kpx.zhijiandao.cn

[Q35] 内连接
来源：http://kjb.gaohongyu789.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ajs.hysaishi.cn

[Q36] 左连接
来源：http://fwn.tianlin.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eac.feifeiyinyue.top

[Q37] 右连接
来源：http://xtj.zycfv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xgd.redwolf501.top

[Q38] 全外连接（PostgreSQL）
来源：http://lwe.cqqwz.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kgx.yj20258888.top

[Q39] 自连接（查上下级）
来源：http://wpo.dianchejie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ugg.wangshuangyany.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://krq.birdmap.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wre.feifeiyinyue.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yfw.yuanzhike.top

[Q41] 多表连接
来源：http://kcy.mhx1999.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mov.0kj1m.cn

JOIN users u ON u.id = o.user_id
来源：http://zdm.9152youxi.cn

JOIN products p ON p.id = o.product_id;
来源：http://xiq.epnwcf.com

[Q42] 连接条件附加过滤
来源：http://smt.tanke756.top

SELECT u.name, o.amount FROM users u
来源：http://oyy.jinyuanbaomall.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uxt.hnqzz.top

[Q43] 标量子查询
来源：http://pka.jinqigufen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hhs.andypj.xyz

[Q44] IN 子查询
来源：http://vid.c1oappe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kis.meibo888.top

[Q45] EXISTS 判断存在
来源：http://hzj.yj20258.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qid.daxiang520.top

[Q46] NOT EXISTS 判断不存在
来源：http://nlf.sxryk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gey.cashguo.top

[Q47] 与平均值比较
来源：http://yxk.zhengqikj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zcq.zhongyouzk.top

[Q48] CTE 公用表表达式
来源：http://dla.fengsongda.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yqs.fzhhl.top

SELECT * FROM t WHERE c > 5;
来源：http://oka.nanxinkj.top

[Q49] 更新单行
来源：http://tpy.wangshuangyany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ruk.zhijiandao.cn

[Q50] 批量更新
来源：http://zbo.xuetiantiany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zen.hnxiangtu.top

[Q51] 用子查询更新
来源：http://pjb.xylfe.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tzd.tianlin.xyz

[Q52] 删除指定行
来源：http://frb.tarul.cn

DELETE FROM users WHERE id = 10;
来源：http://tmp.guowangkeji.top

[Q53] 按条件删除
来源：http://aja.zycfv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fir.fanxiaobao.xyz

[Q54] 清空表
来源：http://ysx.cheryme.top

TRUNCATE TABLE logs;
来源：http://rak.yj20258888.top

[Q55] 排名（并列占位）
来源：http://plq.cucudq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bwv.jinyuanbaomall.cn

[Q56] 密集排名（并列不占位）
来源：http://daa.jiagoushi.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dah.316326.xyz

[Q57] 行号
来源：http://khz.fktsv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nyi.yj202588.top

[Q58] 累计求和
来源：http://dkm.feifeiyinyue.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zoq.cashguo.top

[Q59] 分组内累计
来源：http://zji.daxiang520.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pfb.gaohongyu789.top

[Q60] 取上一行 / 下一行
来源：http://tsx.xinyue.icu

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fkc.ivvv.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mok.ivvv.top

[Q61] 移动平均
来源：http://lry.dianchejie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xvx.ybcxt.top

[Q62] 分组占比
来源：http://xhr.tianlin.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sjs.zhengqikj.top

[Q63] 开启事务
来源：http://kga.tarul.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ura.nanxuanxn.top

[Q64] 提交事务
来源：http://jkk.birdmap.top

COMMIT;
来源：http://nls.shzxlz.cn

[Q65] 回滚事务
来源：http://fgx.0kj1m.cn

ROLLBACK;
来源：http://yqo.meibo888.top

[Q66] 行锁查询
来源：http://wpf.fktsv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jyb.vqdsnc.cn

[Q67] 设置隔离级别
来源：http://zbn.pengpengdd.cyou

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bfj.redwolf501.top

[Q68] 保存点
来源：http://sgv.birdmap.top

SAVEPOINT sp1;
来源：http://tyb.haohaochexian.top

ROLLBACK TO sp1;
来源：http://ayu.guowangkeji.top

[Q69] 查看执行计划
来源：http://ioh.fzhhl.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qkd.quarkkingdee.top

[Q70] 更新统计信息
来源：http://frs.jinqigufen.top

ANALYZE TABLE users;
来源：http://zvg.hnqzz.top

[Q71] 查看建表语句
来源：http://jke.yanxiufei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vet.ywan-chungtsiang.top

[Q72] 查看索引
来源：http://kfx.pengpengdd.cyou

SHOW INDEX FROM users;
来源：http://cmf.bbcook.cn

[Q73] 查看表状态
来源：http://xjg.mhx1999.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tqe.havefunace.top

[Q74] 强制使用索引
来源：http://bqp.pycfn.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://izc.fzhhl.top

[Q75] 日期格式化
来源：http://zoi.aibaodan.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://msx.hywenlv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dts.guannengcc.top

[Q76] 按天统计
来源：http://tvx.jinqigufen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tqx.hongshengwenyu.top

[Q77] 时间加减
来源：http://tes.nanxuanxn.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xjx.dianchejie.cn

[Q78] 当前时间
来源：http://ahc.gotoacloud.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pdz.hongshengwenyu.top

[Q79] 字符串拼接
来源：http://sbv.sxryk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://txa.andypj.xyz

[Q80] 字符串截取
来源：http://oke.hesvh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qhd.c1oappe.top

[Q81] 字符串替换
来源：http://uuh.hfpthk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qjd.jiagoushi.top

[Q82] 字符长度与字节长度
来源：http://puo.gzhubu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zoa.vqdsnc.cn

[Q83] 大小写转换
来源：http://cjk.sjlbkw.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dkn.kuanghao11.cn

[Q84] 去除首尾空格
来源：http://ijr.zhoulong.xyz

SELECT TRIM(name) FROM users;
来源：http://eol.pycfn.com

[Q85] 数值取整
来源：http://qbl.zycfv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sgu.sjlbkw.cn

[Q86] 读取 JSON 字段
来源：http://ler.hammf.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://swr.9152youxi.cn

[Q87] JSON 字段做条件
来源：http://wci.ydzc1.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zik.cashguo.top

[Q88] 行转列（条件聚合）
来源：http://yhc.gzhubu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dcf.cheryme.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uut.wangdashe.top

[Q89] 判断表是否存在
来源：http://zlw.hnxiangtu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://omt.gotoacloud.top

[Q90] 生成序号列
来源：http://byi.guannengcc.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gxo.xinyue.icu

================================================================================
来源：http://ewu.jlsjyb.cn

R. Bash 专题
来源：http://ozd.quarkkingdee.top

================================================================================
来源：http://tcv.guannengcc.top

[R01] shebang 与严格模式
来源：http://tyx.mhx1999.top

#!/usr/bin/env bash
来源：http://luu.bbcook.cn

set -euo pipefail
来源：http://ore.smart0.xyz

[R02] 变量赋值与使用
来源：http://din.vehdjk.com

name="Tom"; echo "$name"
来源：http://zvv.hesvh.cn

[R03] 只读变量
来源：http://kmp.c1oappe.top

readonly PI=3.14
来源：http://vob.chenjidiqi.icu

[R04] 位置参数
来源：http://jlt.shuidangran.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tni.nanxinkj.top

[R05] 参数默认值
来源：http://vkk.hongshengwenyu.top

name="${1:-default}"
来源：http://lcc.snrcjt.cn

[R06] 判断命令是否存在
来源：http://jzz.cucudq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bcd.chenlongwang.top

[R07] if 判断文件
来源：http://jgg.jinqigufen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rin.tian-w.cn

[R08] 数值比较
来源：http://csq.fzhhl.top

if (( a > b )); then echo "a 更大"; fi
来源：http://yce.feifeiyinyue.top

[R09] 字符串比较
来源：http://eva.xziqi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ldm.xziqi.cn

[R10] 正则匹配
来源：http://iug.pycfn.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dlb.jiagoushi.top

[R11] case 多分支
来源：http://wwz.daria6918.cn

case "$1" in
来源：http://qyq.ivvv.top

start) echo "启动" ;;
来源：http://jhk.jlsjyb.cn

stop)  echo "停止" ;;
来源：http://xoz.zhixingplan.top

*)     echo "未知命令" ;;
来源：http://ori.fanxiaobao.xyz

esac
来源：http://gzk.yueranfly.top

[R12] for 遍历文件
来源：http://ybt.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://dgm.gogol.net.cn

[R13] for 计数循环
来源：http://lva.jlsjyb.cn

for i in {1..10}; do echo "$i"; done
来源：http://sco.redwolf501.top

[R14] C 风格 for
来源：http://lhy.zhengqikj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xco.snrcjt.cn

[R15] while 逐行读文件
来源：http://awu.zhiwuduotai.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qaq.shzxlz.cn

[R16] until 等待条件
来源：http://ron.guannengcc.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yfr.cashguo.top

[R17] 数组定义与取值
来源：http://abk.nanxuanxn.top

arr=(a b c); echo "${arr[0]}"
来源：http://wtd.sufxvd.cn

[R18] 遍历数组
来源：http://hjj.jinghuilouyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ris.gzhubu.top

[R19] 数组长度
来源：http://tra.dashuyun.cn

echo "${#arr[@]}"
来源：http://tmu.pycfn.com

[R20] 关联数组（字典）
来源：http://zpy.yonumen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cnj.ydjk.org.cn

[R21] 字符串长度
来源：http://tiv.fktsv.cn

echo "${#s}"
来源：http://ufd.tian-w.cn

[R22] 截取子串
来源：http://qql.jiagoushi.top

echo "${s:0:5}"
来源：http://ntd.hcnkem.com

[R23] 字符串替换
来源：http://hmj.daxiang520.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vbm.gogol.net.cn

[R24] 大小写转换
来源：http://wid.gotoacloud.top

echo "${s^^}"; echo "${s,,}"
来源：http://jfl.aibaodan.cn

[R25] 去后缀 / 去前缀
来源：http://oqs.ydzc1.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://gnt.chenlongwang.top

[R26] 命令替换
来源：http://ybi.sjlbkw.cn

now=$(date +%F); echo "$now"
来源：http://pnr.ydzc1.top

[R27] 算术展开
来源：http://lct.shuidangran.top

echo $((1 + 2 * 3))
来源：http://vzc.wangdashe.top

[R28] 浮点运算
来源：http://owo.haohaochexian.top

echo "scale=2; 10/3" | bc
来源：http://eix.pycfn.com

[R29] 定义函数
来源：http://jdh.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://clg.iojbl.cn

[R30] 函数返回状态码
来源：http://nvi.yanxiufei.cn

f() { return 0; }; f || echo "失败了"
来源：http://jzw.sysykeji.top

[R31] 局部变量
来源：http://kbu.sysykeji.top

f() { local x=1; echo "$x"; }
来源：http://wpn.yueranfly.top

[R32] 参数个数校验
来源：http://nkh.dashuyun.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://str.hongshengwenyu.top

[R33] 捕获错误并提示行号
来源：http://rvj.mhx1999.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ikc.guowangkeji.top

[R34] 退出时清理
来源：http://udw.chenzaomai.com

trap 'rm -f "$tmp"' EXIT
来源：http://bmv.feifeiyinyue.top

[R35] 后台执行并等待
来源：http://psb.quarkkingdee.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zoj.zhiwuduotai.top

[R36] 并发执行多个任务
来源：http://qvn.shanyushiyangtech.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zws.svipenyu.cn

[R37] 把输出赋给变量
来源：http://yzu.hysaishi.cn

files=$(ls -1)
来源：http://zsm.zhongyouzk.top

[R38] 管道串联
来源：http://wit.9152youxi.cn

cat a.txt | grep -i error | wc -l
来源：http://onl.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://uof.bbcook.cn

cmd > out.log 2>&1
来源：http://uxt.xziqi.cn

[R40] 追加写日志
来源：http://kmg.yongpay.top

echo "log" >> out.log
来源：http://bfd.jiagoushi.top

[R41] 丢弃输出
来源：http://lxi.yueranfly.top

cmd >/dev/null 2>&1
来源：http://xjq.wangshuangyany.cn

[R42] 输入重定向
来源：http://kec.xylfe.cn

wc -l < a.txt
来源：http://orw.jianghu66.top

[R43] 按名字查找文件
来源：http://cxu.yongpay.top

find . -name "*.log" -type f
来源：http://abs.jinqigufen.top

[R44] 按修改时间查找
来源：http://tdq.epnwcf.com

find . -mtime -7 -type f
来源：http://jim.ybcxt.top

[R45] 批量删除
来源：http://ysg.hnxiangtu.top

find . -name "*.tmp" -delete
来源：http://hrx.zhoulong.xyz

[R46] 递归替换文件内容
来源：http://ahf.hywenlv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eip.zdqjudy.top

[R47] sed 单行替换
来源：http://zfz.dianchejie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://erc.xylfe.cn

[R48] awk 取指定列
来源：http://tkv.xingfuxueyuan.xyz

awk '{print $1, $3}' a.txt
来源：http://cjr.ehwqpu.com

[R49] awk 带条件
来源：http://sud.redwolf501.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mir.fengsongda.top

[R50] awk 求和
来源：http://dwm.yvedp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mpv.yvedp.cn

[R51] 排序去重取前几
来源：http://ibs.cucudq.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xey.jinqigufen.top

[R52] 统计行数
来源：http://lyo.zdbjq.cn

wc -l a.txt
来源：http://ogt.chenzaomai.com

[R53] 查看文件头与实时尾
来源：http://mys.pengpengdd.cyou

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mkk.fanxiaobao.xyz

[R54] 比较两个文件
来源：http://rwm.fanxiaobao.xyz

diff a.txt b.txt
来源：http://jrt.mhx1999.top

[R55] 压缩与解压
来源：http://qdp.316326.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://com.yueranfly.top

[R56] 远程拷贝
来源：http://xhy.yuxming.cn

scp file user@host:/path/
来源：http://sax.xuetiantiany.cn

[R57] 远程执行命令
来源：http://ath.jiagoushi.top

ssh user@host 'uptime'
来源：http://xdr.chenzaomai.com

[R58] 下载文件
来源：http://uus.sjlbkw.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pli.havefunace.top

[R59] 发 POST JSON
来源：http://zup.mhx1999.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nyk.yangfankeji.com

[R60] 只看 HTTP 状态码
来源：http://uei.zhoulong.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pdn.fktsv.cn

[R61] 磁盘占用
来源：http://lnx.cucudq.cn

df -h;  du -sh *
来源：http://qmw.zhoulong.xyz

[R62] 找最占空间的文件
来源：http://brd.meibo888.top

du -ah . | sort -rh | head -10
来源：http://tpq.sweek.top

[R63] 内存与进程
来源：http://omh.jinyuanbaomall.cn

free -h;  ps aux | grep nginx
来源：http://iln.xylfe.cn

[R64] 结束进程
来源：http://dak.zhongyouzk.top

kill -9 $(pgrep -f app.py)
来源：http://gps.jlsjyb.cn

[R65] 查看端口占用
来源：http://xyx.hfpthk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cjs.jinyuanbaomall.cn

[R66] 定时任务
来源：http://zly.yangfankeji.com

crontab -e;  crontab -l
来源：http://vcp.daxiang520.top

[R67] 生成随机十六进制串
来源：http://uyb.jyoumei.cn

openssl rand -hex 16
来源：http://bnd.tianlin.xyz

[R68] 计算文件校验值
来源：http://ast.xuetiantiany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://clv.9152youxi.cn

[R69] 生成随机密码
来源：http://ftk.fanxiaobao.xyz

head -c 16 /dev/urandom | base64
来源：http://fre.jqgufenzy.top

[R70] 时间戳与互转
来源：http://xpg.hongshengwenyu.top

date +%s;  date -d @1700000000
来源：http://wvy.haohaochexian.top

[R71] 日期格式化
来源：http://wcg.316326.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://apm.yj20258.top

[R72] 等待端口就绪
来源：http://duz.jinyuanbaomall.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ejt.yuanzhike.top

[R73] 分割大日志
来源：http://mug.gaohongyu789.top

split -l 1000 big.log part_
来源：http://kud.dianchejie.cn

[R74] 批量重命名
来源：http://ogi.gaohongyu789.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lfu.shanyushiyangkeji.top

[R75] 导出环境变量
来源：http://ttf.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://qpm.zhengqikj.top

[R76] 使用临时文件
来源：http://dol.jinqigufen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hhy.jiagoushi.top

[R77] 读取用户输入
来源：http://ldp.c1oappe.top

read -rp "请输入: " ans
来源：http://cnm.daxiang520.top

[R78] 交互式菜单
来源：http://sau.cqqwz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zwl.zhongyouzk.top

[R79] 解析命令行选项
来源：http://xpa.ivvv.top


<!-- 参考信息 -->