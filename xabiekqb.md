代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fdf.jqgufenzy.top

) t WHERE rn = 1;
来源：http://pvs.cdnleiting.top

[Q35] 内连接
来源：http://hnu.aibaodan.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://erg.hammf.cn

[Q36] 左连接
来源：http://lqg.fzhhl.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://alz.hnxiangtu.top

[Q37] 右连接
来源：http://ups.jlsjyb.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blz.yuanzhike.top

[Q38] 全外连接（PostgreSQL）
来源：http://udh.ydzc1.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gdp.vehdjk.com

[Q39] 自连接（查上下级）
来源：http://vub.xingfuxueyuan.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://fag.sxryk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aoy.fktsv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vam.guannengcc.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oii.quarkkingdee.top

[Q41] 多表连接
来源：http://hyg.shzxlz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://voa.jqgufenzy.top

JOIN users u ON u.id = o.user_id
来源：http://pgv.redwolf501.top

JOIN products p ON p.id = o.product_id;
来源：http://ktq.yanxiufei.cn

[Q42] 连接条件附加过滤
来源：http://hig.gotoacloud.top

SELECT u.name, o.amount FROM users u
来源：http://zlc.bbcook.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sml.nanxuanxn.top

[Q43] 标量子查询
来源：http://neu.jianghu66.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://htm.shanyushiyangkeji.top

[Q44] IN 子查询
来源：http://lee.dianchejie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bnm.tianlin.xyz

[Q45] EXISTS 判断存在
来源：http://zmd.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://owk.yj20258.top

[Q46] NOT EXISTS 判断不存在
来源：http://thl.xuetiantiany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://npc.jqgfzy.top

[Q47] 与平均值比较
来源：http://jdz.bjfxy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kfh.zhongyouzk.top

[Q48] CTE 公用表表达式
来源：http://rlj.hywenlv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gnm.yuxming.cn

SELECT * FROM t WHERE c > 5;
来源：http://rkg.jinqigufen.top

[Q49] 更新单行
来源：http://bpm.zhengqikj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wpv.nanxinkj.top

[Q50] 批量更新
来源：http://xzm.hfpthk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://npo.cucudq.cn

[Q51] 用子查询更新
来源：http://orx.andypj.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nvz.sjlbkw.cn

[Q52] 删除指定行
来源：http://dpb.yonumen.top

DELETE FROM users WHERE id = 10;
来源：http://bun.shuidangran.top

[Q53] 按条件删除
来源：http://hig.nanxuanxn.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jgk.pycfn.com

[Q54] 清空表
来源：http://kcd.pengpengdd.cyou

TRUNCATE TABLE logs;
来源：http://blj.hesvh.cn

[Q55] 排名（并列占位）
来源：http://ozf.yfazqb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fqa.gaohongyu789.top

[Q56] 密集排名（并列不占位）
来源：http://qjx.yuxming.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vpv.vqdsnc.cn

[Q57] 行号
来源：http://hli.jianghu66.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wua.yj202588.top

[Q58] 累计求和
来源：http://ajy.daria6918.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kpm.yueranfly.top

[Q59] 分组内累计
来源：http://zev.yonumen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dic.fktsv.cn

[Q60] 取上一行 / 下一行
来源：http://rvz.fengsongda.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lei.snrcjt.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mut.ehwqpu.com

[Q61] 移动平均
来源：http://pic.chenzaomai.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oum.andypj.xyz

[Q62] 分组占比
来源：http://uli.jiagoushi.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hff.bbcook.cn

[Q63] 开启事务
来源：http://sks.pycfn.com

START TRANSACTION;                -- 或 BEGIN
来源：http://esx.kuanghao11.cn

[Q64] 提交事务
来源：http://kob.gzhubu.top

COMMIT;
来源：http://tvp.aizwys.cn

[Q65] 回滚事务
来源：http://mdt.jinqigufen.top

ROLLBACK;
来源：http://rsj.fengsongda.top

[Q66] 行锁查询
来源：http://jjo.sweek.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://idm.ppjwa.cn

[Q67] 设置隔离级别
来源：http://cye.316326.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xzj.cheryme.top

[Q68] 保存点
来源：http://lah.chenlongwang.top

SAVEPOINT sp1;
来源：http://ymj.c1oappe.top

ROLLBACK TO sp1;
来源：http://xyk.fzhhl.top

[Q69] 查看执行计划
来源：http://rnc.ybcxt.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hfz.yj20258888.top

[Q70] 更新统计信息
来源：http://hvk.jqgfzy.top

ANALYZE TABLE users;
来源：http://nft.ivvv.top

[Q71] 查看建表语句
来源：http://opf.yongpay.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jio.ppjwa.cn

[Q72] 查看索引
来源：http://fqa.c1oappe.top

SHOW INDEX FROM users;
来源：http://gxy.guowangkeji.top

[Q73] 查看表状态
来源：http://emc.gogol.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bqg.xylfe.cn

[Q74] 强制使用索引
来源：http://ohi.aizwys.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://aom.iojbl.cn

[Q75] 日期格式化
来源：http://ylj.meibo888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zbv.dianchejie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hyt.9152youxi.cn

[Q76] 按天统计
来源：http://kmn.c1oappe.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dhy.tanke756.top

[Q77] 时间加减
来源：http://zkc.zhixingplan.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wvz.ctjpmb.com

[Q78] 当前时间
来源：http://xhd.snrcjt.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://arv.chenlongwang.top

[Q79] 字符串拼接
来源：http://ugb.daria6918.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xnz.hnqzz.top

[Q80] 字符串截取
来源：http://jht.chenzaomai.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://voj.ivvv.top

[Q81] 字符串替换
来源：http://idy.yangfankeji.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://url.dianchejie.cn

[Q82] 字符长度与字节长度
来源：http://iqh.c1oappe.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pql.zhixingplan.top

[Q83] 大小写转换
来源：http://vkw.jinqigfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vge.xuetiantiany.cn

[Q84] 去除首尾空格
来源：http://xjp.yonumen.top

SELECT TRIM(name) FROM users;
来源：http://prh.shuidangran.top

[Q85] 数值取整
来源：http://oip.snrcjt.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qlf.snrcjt.cn

[Q86] 读取 JSON 字段
来源：http://vmx.zhongyouzk.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jio.shanyushiyangtech.top

[Q87] JSON 字段做条件
来源：http://kkl.ybcxt.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eor.guannengcc.top

[Q88] 行转列（条件聚合）
来源：http://eyh.kuanghao11.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cqb.gzhubu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://noe.ywan-chungtsiang.top

[Q89] 判断表是否存在
来源：http://eww.zhengqikj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bfl.0kj1m.cn

[Q90] 生成序号列
来源：http://fcq.fehbvm.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qne.bjfxy.top

================================================================================
来源：http://bov.shuidangran.top

R. Bash 专题
来源：http://tzq.hongshengwenyu.top

================================================================================
来源：http://vak.fanxiaobao.xyz

[R01] shebang 与严格模式
来源：http://nrk.cqqwz.cn

#!/usr/bin/env bash
来源：http://ucp.0kj1m.cn

set -euo pipefail
来源：http://asm.hesvh.cn

[R02] 变量赋值与使用
来源：http://hnk.cqqwz.cn

name="Tom"; echo "$name"
来源：http://arf.cheryme.top

[R03] 只读变量
来源：http://jvh.yangfankeji.com

readonly PI=3.14
来源：http://lrv.yuxming.cn

[R04] 位置参数
来源：http://aga.havefunace.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ozd.nwbrower.top

[R05] 参数默认值
来源：http://szf.vqdsnc.cn

name="${1:-default}"
来源：http://vkz.fanxiaobao.xyz

[R06] 判断命令是否存在
来源：http://uoj.yonumen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kyr.hywenlv.cn

[R07] if 判断文件
来源：http://gff.bbcook.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uwl.ybcxt.top

[R08] 数值比较
来源：http://paw.chenzaomai.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ptv.xuetiantiany.cn

[R09] 字符串比较
来源：http://zsy.hammf.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ava.andypj.xyz

[R10] 正则匹配
来源：http://ily.nwbrower.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://imi.jqgfzy.top

[R11] case 多分支
来源：http://nhv.zdqjudy.top

case "$1" in
来源：http://gif.bjfxy.top

start) echo "启动" ;;
来源：http://czi.hongshengwenyu.top

stop)  echo "停止" ;;
来源：http://gfq.tianlin.xyz

*)     echo "未知命令" ;;
来源：http://hfl.xingfuxueyuan.xyz

esac
来源：http://rri.iojbl.cn

[R12] for 遍历文件
来源：http://mav.vehdjk.com

for f in *.txt; do echo "$f"; done
来源：http://lhy.iojbl.cn

[R13] for 计数循环
来源：http://cll.hongshengwenyu.top

for i in {1..10}; do echo "$i"; done
来源：http://ylz.jinyuanbaomall.cn

[R14] C 风格 for
来源：http://ped.xuetiantiany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iur.zhengqikj.top

[R15] while 逐行读文件
来源：http://awh.yj20258888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xrc.ppjwa.cn

[R16] until 等待条件
来源：http://gnj.svipenyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zgg.c1oappe.top

[R17] 数组定义与取值
来源：http://lsf.xinyue.icu

arr=(a b c); echo "${arr[0]}"
来源：http://icv.nanxinkj.top

[R18] 遍历数组
来源：http://ato.quarkkingdee.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vff.hfpthk.cn

[R19] 数组长度
来源：http://mce.sweek.top

echo "${#arr[@]}"
来源：http://toc.zhengqikj.top

[R20] 关联数组（字典）
来源：http://qfb.316326.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eqm.tanke756.top

[R21] 字符串长度
来源：http://lbe.zhongyouzk.top

echo "${#s}"
来源：http://vur.ehwqpu.com

[R22] 截取子串
来源：http://qvi.uphjek.com

echo "${s:0:5}"
来源：http://kyi.zhongyouzk.top

[R23] 字符串替换
来源：http://hei.gzhubu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fmr.wangshuangyany.cn

[R24] 大小写转换
来源：http://gww.tarul.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rik.yvedp.cn

[R25] 去后缀 / 去前缀
来源：http://btv.tanke756.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://krt.ppjwa.cn

[R26] 命令替换
来源：http://kol.jqgufenzy.top

now=$(date +%F); echo "$now"
来源：http://noz.hongshengwenyu.top

[R27] 算术展开
来源：http://ubl.zhijiandao.cn

echo $((1 + 2 * 3))
来源：http://yzs.yuanzhike.top

[R28] 浮点运算
来源：http://fcu.epnwcf.com

echo "scale=2; 10/3" | bc
来源：http://ptv.zdqjudy.top

[R29] 定义函数
来源：http://ovt.zhixingplan.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ikt.xylfe.cn

[R30] 函数返回状态码
来源：http://rsn.ctjpmb.com

f() { return 0; }; f || echo "失败了"
来源：http://uim.haohaochexian.top

[R31] 局部变量
来源：http://sru.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://lzo.tarul.cn

[R32] 参数个数校验
来源：http://qtm.hongshengwenyu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eyj.ydzc1.top

[R33] 捕获错误并提示行号
来源：http://ksk.sxryk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qlg.smart0.xyz

[R34] 退出时清理
来源：http://dgy.52xcode.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hsm.feifeiyinyue.top

[R35] 后台执行并等待
来源：http://qzv.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xww.mhx1999.top

[R36] 并发执行多个任务
来源：http://mai.jinqigfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ofi.zhoulong.xyz

[R37] 把输出赋给变量
来源：http://ryd.hnxiangtu.top

files=$(ls -1)
来源：http://oyv.shanyushiyangtech.top

[R38] 管道串联
来源：http://bef.cucudq.cn

cat a.txt | grep -i error | wc -l
来源：http://cgj.bjfxy.top

[R39] 重定向标准输出与错误
来源：http://vqq.gogol.net.cn

cmd > out.log 2>&1
来源：http://jkv.gaohongyu789.top

[R40] 追加写日志
来源：http://mas.zhoulong.xyz

echo "log" >> out.log
来源：http://gkc.fengsongda.top

[R41] 丢弃输出
来源：http://qgv.fehbvm.com

cmd >/dev/null 2>&1
来源：http://yhq.52xcode.cn

[R42] 输入重定向
来源：http://gui.hammf.cn

wc -l < a.txt
来源：http://pma.xuanzx.com

[R43] 按名字查找文件
来源：http://jiz.yangfankeji.com

find . -name "*.log" -type f
来源：http://lvb.hnxiangtu.top

[R44] 按修改时间查找
来源：http://ktc.hcnkem.com

find . -mtime -7 -type f
来源：http://cbi.epnwcf.com

[R45] 批量删除
来源：http://psr.chenzaomai.com

find . -name "*.tmp" -delete
来源：http://ibl.jinqigfzy.top

[R46] 递归替换文件内容
来源：http://jep.ybcxt.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bxn.yuxming.cn

[R47] sed 单行替换
来源：http://cqc.fktsv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lyl.jqgufenzy.top

[R48] awk 取指定列
来源：http://zlo.vehdjk.com

awk '{print $1, $3}' a.txt
来源：http://knw.zdqjudy.top

[R49] awk 带条件
来源：http://sjq.meibo888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yvk.gogol.net.cn

[R50] awk 求和
来源：http://hqu.zdbjq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sio.hammf.cn

[R51] 排序去重取前几
来源：http://rfq.uphjek.com

sort a.txt | uniq -c | sort -rn | head
来源：http://fsd.hysaishi.cn

[R52] 统计行数
来源：http://yhn.shanyushiyangtech.top

wc -l a.txt
来源：http://fjk.pycfn.com

[R53] 查看文件头与实时尾
来源：http://sft.fktsv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xsm.tanke756.top

[R54] 比较两个文件
来源：http://ywc.yj202588.top

diff a.txt b.txt
来源：http://rev.dashuyun.cn

[R55] 压缩与解压
来源：http://azt.9152youxi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kbh.jyoumei.cn

[R56] 远程拷贝
来源：http://avf.ivvv.top

scp file user@host:/path/
来源：http://jpm.quarkkingdee.top

[R57] 远程执行命令
来源：http://xvh.zhijiandao.cn

ssh user@host 'uptime'
来源：http://nqu.cheryme.top

[R58] 下载文件
来源：http://rgy.feifeiyinyue.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ext.aibaodan.cn

[R59] 发 POST JSON
来源：http://ymt.birdmap.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tha.andypj.xyz

[R60] 只看 HTTP 状态码
来源：http://zyw.andypj.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dis.jinqigufen.top

[R61] 磁盘占用
来源：http://eur.zhaomingkeji.xyz

df -h;  du -sh *
来源：http://sxr.xziqi.cn

[R62] 找最占空间的文件
来源：http://jsx.yonumen.top

du -ah . | sort -rh | head -10
来源：http://mfa.wangshuangyany.cn

[R63] 内存与进程
来源：http://rbj.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://fjf.yj202588.top

[R64] 结束进程
来源：http://txa.jlsjyb.cn

kill -9 $(pgrep -f app.py)
来源：http://tnc.ywan-chungtsiang.top

[R65] 查看端口占用
来源：http://udv.xingfuxueyuan.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bdm.yongpay.top

[R66] 定时任务
来源：http://luj.zhiwuduotai.top

crontab -e;  crontab -l
来源：http://xdn.iojbl.cn

[R67] 生成随机十六进制串
来源：http://plc.hnxiangtu.top

openssl rand -hex 16
来源：http://vcn.zhengqikj.top

[R68] 计算文件校验值
来源：http://nzr.svipenyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://boe.haohaochexian.top

[R69] 生成随机密码
来源：http://ntg.sxryk.cn

head -c 16 /dev/urandom | base64
来源：http://rem.ivvv.top

[R70] 时间戳与互转
来源：http://rwa.yanxiufei.cn

date +%s;  date -d @1700000000
来源：http://ata.shuidangran.top

[R71] 日期格式化
来源：http://xco.epnwcf.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://knt.guowangkeji.top

[R72] 等待端口就绪
来源：http://wto.zhixingplan.top

until nc -z localhost 3306; do sleep 1; done
来源：http://aif.jqgufenzy.top

[R73] 分割大日志
来源：http://mgj.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://qzh.yuanzhike.top

[R74] 批量重命名
来源：http://hjq.fehbvm.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zpw.meibo888.top

[R75] 导出环境变量
来源：http://vbb.tanke756.top

export PATH="$HOME/bin:$PATH"
来源：http://gks.shzxlz.cn

[R76] 使用临时文件
来源：http://qln.yueranfly.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nsl.dianchejie.cn

[R77] 读取用户输入
来源：http://pba.gaohongyu789.top

read -rp "请输入: " ans
来源：http://gdz.yuxming.cn

[R78] 交互式菜单
来源：http://zty.hywenlv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mog.epnwcf.com

[R79] 解析命令行选项
来源：http://bva.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://glt.tanke756.top

[R80] 查看脚本执行耗时
来源：http://yed.shangyingyoupin.top

time ./run.sh
来源：http://agb.pycfn.com

================================================================================
来源：http://ubi.havefunace.top

S. C / C++ 专题
来源：http://wrf.jinyuanbaomall.cn

================================================================================
来源：http://huy.ydjk.org.cn

[S01] C：Hello World
来源：http://rpo.zhixingplan.top

#include <stdio.h>
来源：http://fqw.9152youxi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uwt.cdnleiting.top

[S02] C：变量与格式化输出
来源：http://rga.wangdashe.top

int a = 10; printf("%d\n", a);
来源：http://vbm.shangyingyoupin.top

[S03] C：读入整数
来源：http://gga.xuetiantiany.cn


<!-- 参考信息 -->