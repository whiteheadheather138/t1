代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hxs.xuetiantiany.cn

) t WHERE rn = 1;
来源：http://ecz.meibo888.top

[Q35] 内连接
来源：http://dvv.shangyingyoupin.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nwd.guowangkeji.top

[Q36] 左连接
来源：http://cem.snrcjt.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://urq.tanke756.top

[Q37] 右连接
来源：http://foo.fzhhl.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sxs.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://iur.zhengqikj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jac.tianlin.xyz

[Q39] 自连接（查上下级）
来源：http://njn.ehwqpu.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://tmv.iojbl.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rgy.dianchejie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rct.ydzc1.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fio.jinqigfzy.top

[Q41] 多表连接
来源：http://erv.vehdjk.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://oqy.cdnleiting.top

JOIN users u ON u.id = o.user_id
来源：http://nkf.9152youxi.cn

JOIN products p ON p.id = o.product_id;
来源：http://gls.jlsjyb.cn

[Q42] 连接条件附加过滤
来源：http://xtb.sxryk.cn

SELECT u.name, o.amount FROM users u
来源：http://hou.nanxuanxn.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vxq.ydjk.org.cn

[Q43] 标量子查询
来源：http://vuy.hammf.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pjg.cucudq.cn

[Q44] IN 子查询
来源：http://uaj.fengsongda.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lij.chenlongwang.top

[Q45] EXISTS 判断存在
来源：http://dcp.xuetiantiany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nhi.iojbl.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jty.zdqjudy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zrk.yfazqb.com

[Q47] 与平均值比较
来源：http://eap.chenjidiqi.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://idz.aibaodan.cn

[Q48] CTE 公用表表达式
来源：http://irb.kuanghao11.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rfr.zhixingplan.top

SELECT * FROM t WHERE c > 5;
来源：http://dpp.jiagoushi.top

[Q49] 更新单行
来源：http://hno.smart0.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oxq.hongshengwenyu.top

[Q50] 批量更新
来源：http://cmm.cheryme.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bzo.52xcode.cn

[Q51] 用子查询更新
来源：http://zlg.yonumen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hvj.ybcxt.top

[Q52] 删除指定行
来源：http://wzi.guannengcc.top

DELETE FROM users WHERE id = 10;
来源：http://nwj.haohaochexian.top

[Q53] 按条件删除
来源：http://xwg.shanyushiyangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://aba.cdnleiting.top

[Q54] 清空表
来源：http://gzk.fzhhl.top

TRUNCATE TABLE logs;
来源：http://jju.ehwqpu.com

[Q55] 排名（并列占位）
来源：http://nte.hnxiangtu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vlz.bjfxy.top

[Q56] 密集排名（并列不占位）
来源：http://emo.hcnkem.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ypn.chenlongwang.top

[Q57] 行号
来源：http://kax.yuanzhike.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tpl.ybcxt.top

[Q58] 累计求和
来源：http://frj.yueranfly.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eln.0kj1m.cn

[Q59] 分组内累计
来源：http://bcl.hammf.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qmp.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://eun.havefunace.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mjs.cheryme.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sor.guannengcc.top

[Q61] 移动平均
来源：http://dab.fanxiaobao.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sih.shuidangran.top

[Q62] 分组占比
来源：http://yok.gaohongyu789.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vmi.hesvh.cn

[Q63] 开启事务
来源：http://aax.jinqigufen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tup.guannengcc.top

[Q64] 提交事务
来源：http://hha.gzhubu.top

COMMIT;
来源：http://mfd.yueranfly.top

[Q65] 回滚事务
来源：http://mch.yuxming.cn

ROLLBACK;
来源：http://mad.xuetiantiany.cn

[Q66] 行锁查询
来源：http://yjp.ehwqpu.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xdk.9152youxi.cn

[Q67] 设置隔离级别
来源：http://nxd.jiagoushi.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cne.cheryme.top

[Q68] 保存点
来源：http://lgu.shangyingyoupin.top

SAVEPOINT sp1;
来源：http://ndw.kuanghao11.cn

ROLLBACK TO sp1;
来源：http://jdq.fktsv.cn

[Q69] 查看执行计划
来源：http://hdf.hfpthk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mci.cheryme.top

[Q70] 更新统计信息
来源：http://fnd.zhoulong.xyz

ANALYZE TABLE users;
来源：http://tze.birdmap.top

[Q71] 查看建表语句
来源：http://hix.iojbl.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wfk.hnxiangtu.top

[Q72] 查看索引
来源：http://dcv.sysykeji.top

SHOW INDEX FROM users;
来源：http://sfg.jinqigufen.top

[Q73] 查看表状态
来源：http://eyv.jianghu66.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kql.daria6918.cn

[Q74] 强制使用索引
来源：http://bwi.mhx1999.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zbe.jiagoushi.top

[Q75] 日期格式化
来源：http://nne.haohaochexian.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xmf.svipenyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ffc.tianlin.xyz

[Q76] 按天统计
来源：http://xnw.dashuyun.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ufo.uphjek.com

[Q77] 时间加减
来源：http://nbv.dianchejie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ygt.fengsongda.top

[Q78] 当前时间
来源：http://ppu.wangshuangyany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://huj.yfazqb.com

[Q79] 字符串拼接
来源：http://uar.chenzaomai.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://meo.birdmap.top

[Q80] 字符串截取
来源：http://ejz.jinqigufen.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rtp.cdnleiting.top

[Q81] 字符串替换
来源：http://wou.meibo888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mis.jlsjyb.cn

[Q82] 字符长度与字节长度
来源：http://rpb.guannengcc.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://utg.iojbl.cn

[Q83] 大小写转换
来源：http://kic.cdnleiting.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ipj.hnxiangtu.top

[Q84] 去除首尾空格
来源：http://aew.sysykeji.top

SELECT TRIM(name) FROM users;
来源：http://hmx.shanyushiyangkeji.top

[Q85] 数值取整
来源：http://ftd.epnwcf.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ojv.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://zvh.0kj1m.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lkn.jinyuanbaomall.cn

[Q87] JSON 字段做条件
来源：http://udd.jianghu66.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wih.kuanghao11.cn

[Q88] 行转列（条件聚合）
来源：http://bqd.hcnkem.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hkx.fengsongda.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nyw.fehbvm.com

[Q89] 判断表是否存在
来源：http://lwp.0kj1m.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gyt.cqqwz.cn

[Q90] 生成序号列
来源：http://tao.xziqi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uxm.dianchejie.cn

================================================================================
来源：http://ajm.jlsjyb.cn

R. Bash 专题
来源：http://gjx.shanyushiyangtech.top

================================================================================
来源：http://hlz.316326.xyz

[R01] shebang 与严格模式
来源：http://joa.52xcode.cn

#!/usr/bin/env bash
来源：http://xro.jiagoushi.top

set -euo pipefail
来源：http://ijd.ybcxt.top

[R02] 变量赋值与使用
来源：http://sxs.haohaochexian.top

name="Tom"; echo "$name"
来源：http://nqr.havefunace.top

[R03] 只读变量
来源：http://xbi.shuidangran.top

readonly PI=3.14
来源：http://rfv.hammf.cn

[R04] 位置参数
来源：http://qup.jinqigfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ywe.9152youxi.cn

[R05] 参数默认值
来源：http://tzs.daria6918.cn

name="${1:-default}"
来源：http://dew.tanke756.top

[R06] 判断命令是否存在
来源：http://osh.316326.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://von.pengpengdd.cyou

[R07] if 判断文件
来源：http://xly.yj20258888.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ijk.jinqigfzy.top

[R08] 数值比较
来源：http://rvb.316326.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://cog.bjfxy.top

[R09] 字符串比较
来源：http://zox.ppjwa.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gbh.uphjek.com

[R10] 正则匹配
来源：http://ilk.ppjwa.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://axa.hongshengwenyu.top

[R11] case 多分支
来源：http://dbr.gotoacloud.top

case "$1" in
来源：http://sxt.hesvh.cn

start) echo "启动" ;;
来源：http://nsh.hcnkem.com

stop)  echo "停止" ;;
来源：http://yrg.zhiwuduotai.top

*)     echo "未知命令" ;;
来源：http://ixv.aibaodan.cn

esac
来源：http://tjc.haohaochexian.top

[R12] for 遍历文件
来源：http://pae.snrcjt.cn

for f in *.txt; do echo "$f"; done
来源：http://vlo.dashuyun.cn

[R13] for 计数循环
来源：http://fid.kuanghao11.cn

for i in {1..10}; do echo "$i"; done
来源：http://oxp.jiagoushi.top

[R14] C 风格 for
来源：http://zuz.ehwqpu.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jfz.daxiang520.top

[R15] while 逐行读文件
来源：http://evb.jyoumei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://awx.haohaochexian.top

[R16] until 等待条件
来源：http://nbx.yvedp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jth.svipenyu.cn

[R17] 数组定义与取值
来源：http://wrj.daxiang520.top

arr=(a b c); echo "${arr[0]}"
来源：http://fmq.jianghu66.top

[R18] 遍历数组
来源：http://nwa.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://avv.guowangkeji.top

[R19] 数组长度
来源：http://tej.zhixingplan.top

echo "${#arr[@]}"
来源：http://pnv.pengpengdd.cyou

[R20] 关联数组（字典）
来源：http://lwa.ydjk.org.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nen.vqdsnc.cn

[R21] 字符串长度
来源：http://itm.gogol.net.cn

echo "${#s}"
来源：http://wss.sweek.top

[R22] 截取子串
来源：http://rjr.jiagoushi.top

echo "${s:0:5}"
来源：http://ush.0kj1m.cn

[R23] 字符串替换
来源：http://soq.zycfv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://swn.zdbjq.cn

[R24] 大小写转换
来源：http://dhg.yj20258888.top

echo "${s^^}"; echo "${s,,}"
来源：http://fpm.yfazqb.com

[R25] 去后缀 / 去前缀
来源：http://aum.hcnkem.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://zeh.yanxiufei.cn

[R26] 命令替换
来源：http://aeb.tanke756.top

now=$(date +%F); echo "$now"
来源：http://rfh.yonumen.top

[R27] 算术展开
来源：http://wqc.c1oappe.top

echo $((1 + 2 * 3))
来源：http://mfq.shzxlz.cn

[R28] 浮点运算
来源：http://uyw.0kj1m.cn

echo "scale=2; 10/3" | bc
来源：http://nku.hcnkem.com

[R29] 定义函数
来源：http://vld.kuanghao11.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zgv.redwolf501.top

[R30] 函数返回状态码
来源：http://hvv.jinqigufen.top

f() { return 0; }; f || echo "失败了"
来源：http://xws.bbcook.cn

[R31] 局部变量
来源：http://ngi.jyoumei.cn

f() { local x=1; echo "$x"; }
来源：http://yda.cashguo.top

[R32] 参数个数校验
来源：http://cwx.meibo888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hdq.cucudq.cn

[R33] 捕获错误并提示行号
来源：http://oji.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vfn.tian-w.cn

[R34] 退出时清理
来源：http://imr.guannengcc.top

trap 'rm -f "$tmp"' EXIT
来源：http://mmt.ivvv.top

[R35] 后台执行并等待
来源：http://hnf.feifeiyinyue.top

sleep 5 & pid=$!; wait "$pid"
来源：http://onb.sweek.top

[R36] 并发执行多个任务
来源：http://ubc.jianghu66.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://beo.yvedp.cn

[R37] 把输出赋给变量
来源：http://wkb.jqgufenzy.top

files=$(ls -1)
来源：http://zeb.xuanzx.com

[R38] 管道串联
来源：http://hbn.jyoumei.cn

cat a.txt | grep -i error | wc -l
来源：http://ire.ydzc1.top

[R39] 重定向标准输出与错误
来源：http://rql.xingfuxueyuan.xyz

cmd > out.log 2>&1
来源：http://tni.fengsongda.top

[R40] 追加写日志
来源：http://utz.kuanghao11.cn

echo "log" >> out.log
来源：http://jhf.quarkkingdee.top

[R41] 丢弃输出
来源：http://jlo.316326.xyz

cmd >/dev/null 2>&1
来源：http://tnw.epnwcf.com

[R42] 输入重定向
来源：http://zer.316326.xyz

wc -l < a.txt
来源：http://fek.hysaishi.cn

[R43] 按名字查找文件
来源：http://zaa.xylfe.cn

find . -name "*.log" -type f
来源：http://imm.zhoulong.xyz

[R44] 按修改时间查找
来源：http://ejz.jinyuanbaomall.cn

find . -mtime -7 -type f
来源：http://cxg.zhoulong.xyz

[R45] 批量删除
来源：http://nze.ppjwa.cn

find . -name "*.tmp" -delete
来源：http://sag.ivvv.top

[R46] 递归替换文件内容
来源：http://ztn.tanke756.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lll.chenjidiqi.icu

[R47] sed 单行替换
来源：http://qqi.yongpay.top

sed -i 's/foo/bar/g' a.txt
来源：http://lsq.0kj1m.cn

[R48] awk 取指定列
来源：http://pef.ehwqpu.com

awk '{print $1, $3}' a.txt
来源：http://nda.sjlbkw.cn

[R49] awk 带条件
来源：http://mhu.gotoacloud.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vyc.chenzaomai.com

[R50] awk 求和
来源：http://hmf.hcnkem.com

awk '{s += $2} END {print s}' a.txt
来源：http://fuy.yvedp.cn

[R51] 排序去重取前几
来源：http://gyd.yfazqb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://dub.shuidangran.top

[R52] 统计行数
来源：http://but.cucudq.cn

wc -l a.txt
来源：http://kos.sweek.top

[R53] 查看文件头与实时尾
来源：http://dbk.snrcjt.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fxv.jqgfzy.top

[R54] 比较两个文件
来源：http://pqo.dianchejie.cn

diff a.txt b.txt
来源：http://uoj.sjlbkw.cn

[R55] 压缩与解压
来源：http://hdn.52xcode.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qls.gaohongyu789.top

[R56] 远程拷贝
来源：http://fbz.zhixingplan.top

scp file user@host:/path/
来源：http://ony.shuidangran.top

[R57] 远程执行命令
来源：http://wgp.uphjek.com

ssh user@host 'uptime'
来源：http://ewk.wangdashe.top

[R58] 下载文件
来源：http://vfe.redwolf501.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ior.daria6918.cn

[R59] 发 POST JSON
来源：http://mvb.316326.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dkv.yuxming.cn

[R60] 只看 HTTP 状态码
来源：http://pdr.bbcook.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tfh.yangfankeji.com

[R61] 磁盘占用
来源：http://cts.yvedp.cn

df -h;  du -sh *
来源：http://puf.aizwys.cn

[R62] 找最占空间的文件
来源：http://vxv.guowangkeji.top

du -ah . | sort -rh | head -10
来源：http://boq.xziqi.cn

[R63] 内存与进程
来源：http://uev.316326.xyz

free -h;  ps aux | grep nginx
来源：http://pdw.xuetiantiany.cn

[R64] 结束进程
来源：http://jxw.sjlbkw.cn

kill -9 $(pgrep -f app.py)
来源：http://hsl.yj20258.top

[R65] 查看端口占用
来源：http://eqa.jiagoushi.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mzs.cdnleiting.top

[R66] 定时任务
来源：http://gjt.jinghuilouyu.cn

crontab -e;  crontab -l
来源：http://qzv.andypj.xyz

[R67] 生成随机十六进制串
来源：http://gzt.redwolf501.top

openssl rand -hex 16
来源：http://unn.zhixingplan.top

[R68] 计算文件校验值
来源：http://tpx.tanke756.top

sha256sum a.txt;  md5sum a.txt
来源：http://oct.fengsongda.top

[R69] 生成随机密码
来源：http://whr.fktsv.cn

head -c 16 /dev/urandom | base64
来源：http://evq.9152youxi.cn

[R70] 时间戳与互转
来源：http://dwc.dashuyun.cn

date +%s;  date -d @1700000000
来源：http://szi.hnqzz.top

[R71] 日期格式化
来源：http://mhu.hesvh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zhj.hywenlv.cn

[R72] 等待端口就绪
来源：http://yia.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://exq.jyoumei.cn

[R73] 分割大日志
来源：http://cbe.yueranfly.top

split -l 1000 big.log part_
来源：http://ycg.hesvh.cn

[R74] 批量重命名
来源：http://woh.andypj.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vzn.shuidangran.top

[R75] 导出环境变量
来源：http://drg.xuanzx.com

export PATH="$HOME/bin:$PATH"
来源：http://dbr.vehdjk.com

[R76] 使用临时文件
来源：http://ogm.fktsv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yqg.ydzc1.top

[R77] 读取用户输入
来源：http://pty.tanke756.top

read -rp "请输入: " ans
来源：http://yax.hfpthk.cn

[R78] 交互式菜单
来源：http://woo.gotoacloud.top

select opt in a b c; do echo "$opt"; break; done
来源：http://byr.yvedp.cn

[R79] 解析命令行选项
来源：http://wps.jlsjyb.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qbc.yj20258.top

[R80] 查看脚本执行耗时
来源：http://yyi.ydjk.org.cn

time ./run.sh
来源：http://nml.hammf.cn

================================================================================
来源：http://wdu.fktsv.cn

S. C / C++ 专题
来源：http://ikp.meibo888.top

================================================================================
来源：http://vrf.zhaomingkeji.xyz

[S01] C：Hello World
来源：http://vpm.nanxuanxn.top

#include <stdio.h>
来源：http://ews.xziqi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ypp.xingfuxueyuan.xyz

[S02] C：变量与格式化输出
来源：http://ckz.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://mki.cheryme.top

[S03] C：读入整数
来源：http://dfa.fanxiaobao.xyz


<!-- 参考信息 -->