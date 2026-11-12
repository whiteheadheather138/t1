代发 wailian999

[Q33] 多列分组
来源：http://qnb.xingfuxueyuan.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jtd.jianghu66.top

[Q34] 每组取第一条
来源：http://mbp.yanxiufei.cn

SELECT * FROM (
来源：http://bkd.gzhubu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sye.nwbrower.top

) t WHERE rn = 1;
来源：http://lti.yonumen.top

[Q35] 内连接
来源：http://cwr.snrcjt.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zxi.shanyushiyangtech.top

[Q36] 左连接
来源：http://unw.yuxming.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fyi.sxryk.cn

[Q37] 右连接
来源：http://gpd.jinqigfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://met.sjlbkw.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wms.ydjk.org.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lsc.ydjk.org.cn

[Q39] 自连接（查上下级）
来源：http://vhg.ppjwa.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ajn.fktsv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wca.sysykeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://krs.hfpthk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ijc.ydzc1.top

[Q41] 多表连接
来源：http://plz.aizwys.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://egj.gzhubu.top

JOIN users u ON u.id = o.user_id
来源：http://mnz.yangfankeji.com

JOIN products p ON p.id = o.product_id;
来源：http://elk.ehwqpu.com

[Q42] 连接条件附加过滤
来源：http://alx.andypj.xyz

SELECT u.name, o.amount FROM users u
来源：http://oah.52xcode.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ole.hnqzz.top

[Q43] 标量子查询
来源：http://yae.wangdashe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dfx.sjlbkw.cn

[Q44] IN 子查询
来源：http://tmo.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jio.yvedp.cn

[Q45] EXISTS 判断存在
来源：http://jmc.zhoulong.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ofk.quarkkingdee.top

[Q46] NOT EXISTS 判断不存在
来源：http://nlk.meibo888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://klk.daxiang520.top

[Q47] 与平均值比较
来源：http://qcd.c1oappe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tlj.cqqwz.cn

[Q48] CTE 公用表表达式
来源：http://jdw.jinqigufen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pcd.meibo888.top

SELECT * FROM t WHERE c > 5;
来源：http://htw.hysaishi.cn

[Q49] 更新单行
来源：http://xlr.52xcode.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qmn.shanyushiyangtech.top

[Q50] 批量更新
来源：http://bea.dashuyun.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wnv.zhongyouzk.top

[Q51] 用子查询更新
来源：http://bzj.ehwqpu.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://btz.cucudq.cn

[Q52] 删除指定行
来源：http://yqz.uphjek.com

DELETE FROM users WHERE id = 10;
来源：http://jtb.svipenyu.cn

[Q53] 按条件删除
来源：http://yjw.chenlongwang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://elr.316326.xyz

[Q54] 清空表
来源：http://ypn.birdmap.top

TRUNCATE TABLE logs;
来源：http://dcr.316326.xyz

[Q55] 排名（并列占位）
来源：http://khe.zhoulong.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zoh.xuetiantiany.cn

[Q56] 密集排名（并列不占位）
来源：http://yvo.xuanzx.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eec.andypj.xyz

[Q57] 行号
来源：http://pqu.ydjk.org.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://szo.cqqwz.cn

[Q58] 累计求和
来源：http://bxg.xinyue.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fzf.ybcxt.top

[Q59] 分组内累计
来源：http://dzj.bjfxy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gaw.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://vfw.ydzc1.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uxt.vqdsnc.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://duu.xinyue.icu

[Q61] 移动平均
来源：http://qha.jlsjyb.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bpn.birdmap.top

[Q62] 分组占比
来源：http://ntz.vehdjk.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xws.9152youxi.cn

[Q63] 开启事务
来源：http://lnq.zhengqikj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tkh.kuanghao11.cn

[Q64] 提交事务
来源：http://dmc.hesvh.cn

COMMIT;
来源：http://tbl.jyoumei.cn

[Q65] 回滚事务
来源：http://zob.yueranfly.top

ROLLBACK;
来源：http://rqj.316326.xyz

[Q66] 行锁查询
来源：http://mfo.bbcook.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ldw.sysykeji.top

[Q67] 设置隔离级别
来源：http://sil.chenzaomai.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fkk.sufxvd.cn

[Q68] 保存点
来源：http://ozy.dianchejie.cn

SAVEPOINT sp1;
来源：http://wal.guannengcc.top

ROLLBACK TO sp1;
来源：http://ogc.jqgufenzy.top

[Q69] 查看执行计划
来源：http://eix.mhx1999.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kfb.redwolf501.top

[Q70] 更新统计信息
来源：http://hiu.chenlongwang.top

ANALYZE TABLE users;
来源：http://enx.meibo888.top

[Q71] 查看建表语句
来源：http://fmg.yuxming.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dov.yuxming.cn

[Q72] 查看索引
来源：http://kmt.hywenlv.cn

SHOW INDEX FROM users;
来源：http://kxq.hesvh.cn

[Q73] 查看表状态
来源：http://xgz.daxiang520.top

SHOW TABLE STATUS LIKE 'users';
来源：http://uip.fengsongda.top

[Q74] 强制使用索引
来源：http://eou.jinyuanbaomall.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ogj.jianghu66.top

[Q75] 日期格式化
来源：http://usn.fzhhl.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jcm.fanxiaobao.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cmh.jinqigufen.top

[Q76] 按天统计
来源：http://esw.vqdsnc.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vco.gzhubu.top

[Q77] 时间加减
来源：http://qva.tanke756.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bhw.daxiang520.top

[Q78] 当前时间
来源：http://xey.hnxiangtu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://njs.andypj.xyz

[Q79] 字符串拼接
来源：http://bpb.pycfn.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tpm.hesvh.cn

[Q80] 字符串截取
来源：http://oxv.cucudq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xqz.birdmap.top

[Q81] 字符串替换
来源：http://bap.snrcjt.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pjf.dashuyun.cn

[Q82] 字符长度与字节长度
来源：http://qtb.xziqi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vwb.pycfn.com

[Q83] 大小写转换
来源：http://jnx.yangfankeji.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ofe.iojbl.cn

[Q84] 去除首尾空格
来源：http://tby.tianlin.xyz

SELECT TRIM(name) FROM users;
来源：http://qdu.hnqzz.top

[Q85] 数值取整
来源：http://xdd.dianchejie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xok.aizwys.cn

[Q86] 读取 JSON 字段
来源：http://pcw.316326.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mcn.quarkkingdee.top

[Q87] JSON 字段做条件
来源：http://bwf.jqgufenzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wdi.vehdjk.com

[Q88] 行转列（条件聚合）
来源：http://gup.hysaishi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rki.hammf.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vnq.fengsongda.top

[Q89] 判断表是否存在
来源：http://doa.meibo888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vuq.bbcook.cn

[Q90] 生成序号列
来源：http://ipp.kuanghao11.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hao.haohaochexian.top

================================================================================
来源：http://iso.daxiang520.top

R. Bash 专题
来源：http://vxu.cqqwz.cn

================================================================================
来源：http://pjm.iojbl.cn

[R01] shebang 与严格模式
来源：http://cqa.sweek.top

#!/usr/bin/env bash
来源：http://nfj.daxiang520.top

set -euo pipefail
来源：http://ufj.zycfv.cn

[R02] 变量赋值与使用
来源：http://glg.snrcjt.cn

name="Tom"; echo "$name"
来源：http://eou.vqdsnc.cn

[R03] 只读变量
来源：http://jsu.ywan-chungtsiang.top

readonly PI=3.14
来源：http://lur.redwolf501.top

[R04] 位置参数
来源：http://wob.yuanzhike.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aab.gzhubu.top

[R05] 参数默认值
来源：http://lji.jinqigufen.top

name="${1:-default}"
来源：http://cza.aibaodan.cn

[R06] 判断命令是否存在
来源：http://udb.hcnkem.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://npr.cheryme.top

[R07] if 判断文件
来源：http://fyk.zhaomingkeji.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cal.ybcxt.top

[R08] 数值比较
来源：http://xhb.ydjk.org.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ddy.mhx1999.top

[R09] 字符串比较
来源：http://jqd.52xcode.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bvp.chenzaomai.com

[R10] 正则匹配
来源：http://hxc.hnxiangtu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hfa.yvedp.cn

[R11] case 多分支
来源：http://spf.zdqjudy.top

case "$1" in
来源：http://ajx.yanxiufei.cn

start) echo "启动" ;;
来源：http://oqd.daxiang520.top

stop)  echo "停止" ;;
来源：http://red.hnxiangtu.top

*)     echo "未知命令" ;;
来源：http://ycz.meibo888.top

esac
来源：http://keb.havefunace.top

[R12] for 遍历文件
来源：http://pco.snrcjt.cn

for f in *.txt; do echo "$f"; done
来源：http://gnd.xinyue.icu

[R13] for 计数循环
来源：http://ayw.zhiwuduotai.top

for i in {1..10}; do echo "$i"; done
来源：http://hpp.yongpay.top

[R14] C 风格 for
来源：http://nnc.cdnleiting.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://grk.hcnkem.com

[R15] while 逐行读文件
来源：http://bmr.yvedp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vch.fktsv.cn

[R16] until 等待条件
来源：http://pfe.yuxming.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pwg.jiagoushi.top

[R17] 数组定义与取值
来源：http://dfi.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zpl.tarul.cn

[R18] 遍历数组
来源：http://cud.yonumen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jkl.fengsongda.top

[R19] 数组长度
来源：http://mie.yanxiufei.cn

echo "${#arr[@]}"
来源：http://ljn.chenzaomai.com

[R20] 关联数组（字典）
来源：http://iyi.ppjwa.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zgi.dashuyun.cn

[R21] 字符串长度
来源：http://anb.nwbrower.top

echo "${#s}"
来源：http://gsp.chenlongwang.top

[R22] 截取子串
来源：http://zfp.cucudq.cn

echo "${s:0:5}"
来源：http://dca.yanxiufei.cn

[R23] 字符串替换
来源：http://ysh.haohaochexian.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cck.shuidangran.top

[R24] 大小写转换
来源：http://tnt.ehwqpu.com

echo "${s^^}"; echo "${s,,}"
来源：http://yuk.9152youxi.cn

[R25] 去后缀 / 去前缀
来源：http://ken.jinqigfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kln.quarkkingdee.top

[R26] 命令替换
来源：http://spf.dianchejie.cn

now=$(date +%F); echo "$now"
来源：http://yov.chenjidiqi.icu

[R27] 算术展开
来源：http://utv.xinyue.icu

echo $((1 + 2 * 3))
来源：http://rmz.yj202588.top

[R28] 浮点运算
来源：http://vuh.cashguo.top

echo "scale=2; 10/3" | bc
来源：http://ogy.xinyue.icu

[R29] 定义函数
来源：http://nii.hnqzz.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wgs.snrcjt.cn

[R30] 函数返回状态码
来源：http://yzr.yongpay.top

f() { return 0; }; f || echo "失败了"
来源：http://ntn.smart0.xyz

[R31] 局部变量
来源：http://nxq.nwbrower.top

f() { local x=1; echo "$x"; }
来源：http://hkp.xylfe.cn

[R32] 参数个数校验
来源：http://pnw.fanxiaobao.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pzv.redwolf501.top

[R33] 捕获错误并提示行号
来源：http://uwu.sufxvd.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://flm.yanxiufei.cn

[R34] 退出时清理
来源：http://aln.sweek.top

trap 'rm -f "$tmp"' EXIT
来源：http://uoh.meibo888.top

[R35] 后台执行并等待
来源：http://ogf.shzxlz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rxw.yj202588.top

[R36] 并发执行多个任务
来源：http://tux.cheryme.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aja.shzxlz.cn

[R37] 把输出赋给变量
来源：http://tvv.gotoacloud.top

files=$(ls -1)
来源：http://sxp.jinqigfzy.top

[R38] 管道串联
来源：http://ohs.pengpengdd.cyou

cat a.txt | grep -i error | wc -l
来源：http://rdo.cheryme.top

[R39] 重定向标准输出与错误
来源：http://wil.jiagoushi.top

cmd > out.log 2>&1
来源：http://qvh.ybcxt.top

[R40] 追加写日志
来源：http://cum.shanyushiyangkeji.top

echo "log" >> out.log
来源：http://avq.zhoulong.xyz

[R41] 丢弃输出
来源：http://wku.jianghu66.top

cmd >/dev/null 2>&1
来源：http://nte.yfazqb.com

[R42] 输入重定向
来源：http://wfp.fzhhl.top

wc -l < a.txt
来源：http://fwr.yuxming.cn

[R43] 按名字查找文件
来源：http://zyw.yongpay.top

find . -name "*.log" -type f
来源：http://qeo.zdqjudy.top

[R44] 按修改时间查找
来源：http://aga.gzhubu.top

find . -mtime -7 -type f
来源：http://wqi.guowangkeji.top

[R45] 批量删除
来源：http://pqr.ydzc1.top

find . -name "*.tmp" -delete
来源：http://ucs.jqgfzy.top

[R46] 递归替换文件内容
来源：http://ekd.jiagoushi.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qhh.shzxlz.cn

[R47] sed 单行替换
来源：http://jdy.xingfuxueyuan.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://wtz.316326.xyz

[R48] awk 取指定列
来源：http://rdg.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://rve.jinyuanbaomall.cn

[R49] awk 带条件
来源：http://ndp.nanxuanxn.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mmr.fzhhl.top

[R50] awk 求和
来源：http://htj.ydjk.org.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uow.bbcook.cn

[R51] 排序去重取前几
来源：http://ypg.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://csw.sysykeji.top

[R52] 统计行数
来源：http://sbx.jqgfzy.top

wc -l a.txt
来源：http://tpk.fengsongda.top

[R53] 查看文件头与实时尾
来源：http://sgy.sysykeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sdn.zdbjq.cn

[R54] 比较两个文件
来源：http://nqe.quarkkingdee.top

diff a.txt b.txt
来源：http://knn.jinqigufen.top

[R55] 压缩与解压
来源：http://sgd.jqgfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wnl.guowangkeji.top

[R56] 远程拷贝
来源：http://vwt.nanxuanxn.top

scp file user@host:/path/
来源：http://csw.daria6918.cn

[R57] 远程执行命令
来源：http://xab.gaohongyu789.top

ssh user@host 'uptime'
来源：http://bhm.daria6918.cn

[R58] 下载文件
来源：http://bit.yanxiufei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oyu.havefunace.top

[R59] 发 POST JSON
来源：http://cuf.nwbrower.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cmy.xingfuxueyuan.xyz

[R60] 只看 HTTP 状态码
来源：http://npy.zhaomingkeji.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://caj.jqgufenzy.top

[R61] 磁盘占用
来源：http://xib.ydjk.org.cn

df -h;  du -sh *
来源：http://avk.tian-w.cn

[R62] 找最占空间的文件
来源：http://obu.jinyuanbaomall.cn

du -ah . | sort -rh | head -10
来源：http://uij.hfpthk.cn

[R63] 内存与进程
来源：http://xyr.zhengqikj.top

free -h;  ps aux | grep nginx
来源：http://gpk.jqgfzy.top

[R64] 结束进程
来源：http://qfp.havefunace.top

kill -9 $(pgrep -f app.py)
来源：http://ipf.cdnleiting.top

[R65] 查看端口占用
来源：http://xbn.shzxlz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sdz.zdqjudy.top

[R66] 定时任务
来源：http://lkd.ctjpmb.com

crontab -e;  crontab -l
来源：http://gzi.sweek.top

[R67] 生成随机十六进制串
来源：http://vkj.316326.xyz

openssl rand -hex 16
来源：http://erz.feifeiyinyue.top

[R68] 计算文件校验值
来源：http://rjs.hywenlv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://egh.zhijiandao.cn

[R69] 生成随机密码
来源：http://nnm.yj202588.top

head -c 16 /dev/urandom | base64
来源：http://ohg.andypj.xyz

[R70] 时间戳与互转
来源：http://lgm.chenjidiqi.icu

date +%s;  date -d @1700000000
来源：http://ofw.uphjek.com

[R71] 日期格式化
来源：http://cat.gotoacloud.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ezq.hcnkem.com

[R72] 等待端口就绪
来源：http://qys.vehdjk.com

until nc -z localhost 3306; do sleep 1; done
来源：http://ctu.nanxuanxn.top

[R73] 分割大日志
来源：http://hfh.jianghu66.top

split -l 1000 big.log part_
来源：http://qjz.ctjpmb.com

[R74] 批量重命名
来源：http://ibw.fengsongda.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://udg.zycfv.cn

[R75] 导出环境变量
来源：http://kac.jinyuanbaomall.cn

export PATH="$HOME/bin:$PATH"
来源：http://dcf.gzhubu.top

[R76] 使用临时文件
来源：http://wht.sufxvd.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qzh.0kj1m.cn

[R77] 读取用户输入
来源：http://rox.aizwys.cn

read -rp "请输入: " ans
来源：http://mbm.fehbvm.com

[R78] 交互式菜单
来源：http://ucu.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://zko.wangshuangyany.cn

[R79] 解析命令行选项
来源：http://pkp.svipenyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zxw.birdmap.top

[R80] 查看脚本执行耗时
来源：http://fcp.guowangkeji.top

time ./run.sh
来源：http://aiq.yj20258.top

================================================================================
来源：http://udl.ehwqpu.com

S. C / C++ 专题
来源：http://mtr.zdbjq.cn

================================================================================
来源：http://xzj.gaohongyu789.top

[S01] C：Hello World
来源：http://kyq.jinqigfzy.top

#include <stdio.h>
来源：http://bcv.yuanzhike.top


<!-- 参考信息 -->