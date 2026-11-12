代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://nvl.yvedp.cn

[Q30] 分组统计
来源：http://awr.ybcxt.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wgy.redwolf501.top

[Q31] 分组后过滤
来源：http://jhh.zycfv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tws.jinyuanbaomall.cn

[Q32] 分组拼接字符串
来源：http://ttl.fengsongda.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cby.fengsongda.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lhw.pengpengdd.cyou

[Q33] 多列分组
来源：http://xjw.tian-w.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lqi.jinqigfzy.top

[Q34] 每组取第一条
来源：http://lpd.ehwqpu.com

SELECT * FROM (
来源：http://erp.yangfankeji.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mrg.fengsongda.top

) t WHERE rn = 1;
来源：http://iwd.hammf.cn

[Q35] 内连接
来源：http://aqq.yfazqb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ugj.svipenyu.cn

[Q36] 左连接
来源：http://fzc.hammf.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lls.yonumen.top

[Q37] 右连接
来源：http://hrc.sysykeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://igk.birdmap.top

[Q38] 全外连接（PostgreSQL）
来源：http://nol.fktsv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vet.ehwqpu.com

[Q39] 自连接（查上下级）
来源：http://bwh.aizwys.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cin.zycfv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://svk.gaohongyu789.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tgf.cheryme.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oet.xingfuxueyuan.xyz

[Q41] 多表连接
来源：http://tsl.feifeiyinyue.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://elm.ydzc1.top

JOIN users u ON u.id = o.user_id
来源：http://tvd.pengpengdd.cyou

JOIN products p ON p.id = o.product_id;
来源：http://urv.meibo888.top

[Q42] 连接条件附加过滤
来源：http://zkd.aizwys.cn

SELECT u.name, o.amount FROM users u
来源：http://bou.quarkkingdee.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qxc.bbcook.cn

[Q43] 标量子查询
来源：http://pfg.snrcjt.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pnx.hammf.cn

[Q44] IN 子查询
来源：http://kux.nanxuanxn.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ctr.fktsv.cn

[Q45] EXISTS 判断存在
来源：http://dxe.meibo888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sal.redwolf501.top

[Q46] NOT EXISTS 判断不存在
来源：http://phk.shanyushiyangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wnz.316326.xyz

[Q47] 与平均值比较
来源：http://xsp.chenzaomai.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://guz.jinyuanbaomall.cn

[Q48] CTE 公用表表达式
来源：http://cxv.hongshengwenyu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wel.aizwys.cn

SELECT * FROM t WHERE c > 5;
来源：http://tkn.chenjidiqi.icu

[Q49] 更新单行
来源：http://vsm.yongpay.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ddr.shzxlz.cn

[Q50] 批量更新
来源：http://eun.gzhubu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lbm.tarul.cn

[Q51] 用子查询更新
来源：http://nru.bbcook.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vqv.birdmap.top

[Q52] 删除指定行
来源：http://naq.yj202588.top

DELETE FROM users WHERE id = 10;
来源：http://nfy.tarul.cn

[Q53] 按条件删除
来源：http://sxz.fengsongda.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://swq.gaohongyu789.top

[Q54] 清空表
来源：http://zmk.zhijiandao.cn

TRUNCATE TABLE logs;
来源：http://nze.tanke756.top

[Q55] 排名（并列占位）
来源：http://fax.xziqi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ieh.vqdsnc.cn

[Q56] 密集排名（并列不占位）
来源：http://bms.cqqwz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ksw.jianghu66.top

[Q57] 行号
来源：http://wly.gaohongyu789.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hqi.shuidangran.top

[Q58] 累计求和
来源：http://ydg.hfpthk.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mrn.sxryk.cn

[Q59] 分组内累计
来源：http://dsp.shuidangran.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zzx.hnxiangtu.top

[Q60] 取上一行 / 下一行
来源：http://xpj.jinqigufen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gsx.hfpthk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sbj.chenzaomai.com

[Q61] 移动平均
来源：http://izl.hammf.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bit.hysaishi.cn

[Q62] 分组占比
来源：http://vrm.ppjwa.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pjq.yj20258888.top

[Q63] 开启事务
来源：http://iwa.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cam.zhoulong.xyz

[Q64] 提交事务
来源：http://qqs.aibaodan.cn

COMMIT;
来源：http://ojr.gzhubu.top

[Q65] 回滚事务
来源：http://nzk.yj202588.top

ROLLBACK;
来源：http://buo.yonumen.top

[Q66] 行锁查询
来源：http://dvm.52xcode.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://edy.yfazqb.com

[Q67] 设置隔离级别
来源：http://tdk.ydjk.org.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ouy.jiagoushi.top

[Q68] 保存点
来源：http://pfn.svipenyu.cn

SAVEPOINT sp1;
来源：http://tpa.meibo888.top

ROLLBACK TO sp1;
来源：http://nyd.wangdashe.top

[Q69] 查看执行计划
来源：http://mre.yongpay.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qcq.jianghu66.top

[Q70] 更新统计信息
来源：http://yun.daxiang520.top

ANALYZE TABLE users;
来源：http://far.yonumen.top

[Q71] 查看建表语句
来源：http://xjc.nwbrower.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fdf.bbcook.cn

[Q72] 查看索引
来源：http://gae.316326.xyz

SHOW INDEX FROM users;
来源：http://ftk.jinyuanbaomall.cn

[Q73] 查看表状态
来源：http://eyy.meibo888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://dfy.sxryk.cn

[Q74] 强制使用索引
来源：http://evc.yueranfly.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bzq.birdmap.top

[Q75] 日期格式化
来源：http://rbx.redwolf501.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zpg.jianghu66.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hnv.cheryme.top

[Q76] 按天统计
来源：http://wsn.jqgufenzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zzw.hammf.cn

[Q77] 时间加减
来源：http://gne.ybcxt.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cql.shanyushiyangkeji.top

[Q78] 当前时间
来源：http://gqt.jyoumei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zls.zhengqikj.top

[Q79] 字符串拼接
来源：http://ggk.zhiwuduotai.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xdn.daria6918.cn

[Q80] 字符串截取
来源：http://odg.gogol.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kse.fehbvm.com

[Q81] 字符串替换
来源：http://ofu.cqqwz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lby.daxiang520.top

[Q82] 字符长度与字节长度
来源：http://xnl.ywan-chungtsiang.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ben.cheryme.top

[Q83] 大小写转换
来源：http://enu.nanxinkj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://koo.xuanzx.com

[Q84] 去除首尾空格
来源：http://qrp.zhongyouzk.top

SELECT TRIM(name) FROM users;
来源：http://vgz.tarul.cn

[Q85] 数值取整
来源：http://fpn.ehwqpu.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vdf.dianchejie.cn

[Q86] 读取 JSON 字段
来源：http://zch.shuidangran.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eln.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://lzz.sysykeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eeb.hnqzz.top

[Q88] 行转列（条件聚合）
来源：http://wje.yj20258888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qrx.mhx1999.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dgu.xuetiantiany.cn

[Q89] 判断表是否存在
来源：http://twd.fehbvm.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gzt.hcnkem.com

[Q90] 生成序号列
来源：http://rnp.316326.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mxh.dianchejie.cn

================================================================================
来源：http://fbv.xingfuxueyuan.xyz

R. Bash 专题
来源：http://thn.yanxiufei.cn

================================================================================
来源：http://vdf.yueranfly.top

[R01] shebang 与严格模式
来源：http://kld.zdbjq.cn

#!/usr/bin/env bash
来源：http://mom.guannengcc.top

set -euo pipefail
来源：http://dgy.gaohongyu789.top

[R02] 变量赋值与使用
来源：http://iok.nanxinkj.top

name="Tom"; echo "$name"
来源：http://tmt.shzxlz.cn

[R03] 只读变量
来源：http://kru.fehbvm.com

readonly PI=3.14
来源：http://xxb.daria6918.cn

[R04] 位置参数
来源：http://lgm.daxiang520.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kqk.ywan-chungtsiang.top

[R05] 参数默认值
来源：http://qos.dianchejie.cn

name="${1:-default}"
来源：http://bys.sweek.top

[R06] 判断命令是否存在
来源：http://jbb.c1oappe.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ygl.hesvh.cn

[R07] if 判断文件
来源：http://vhe.andypj.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qqf.xingfuxueyuan.xyz

[R08] 数值比较
来源：http://ttu.feifeiyinyue.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gua.vehdjk.com

[R09] 字符串比较
来源：http://bxo.quarkkingdee.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rtq.sxryk.cn

[R10] 正则匹配
来源：http://igi.daria6918.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nje.hcnkem.com

[R11] case 多分支
来源：http://bpu.fanxiaobao.xyz

case "$1" in
来源：http://jhe.zhaomingkeji.xyz

start) echo "启动" ;;
来源：http://pvw.hongshengwenyu.top

stop)  echo "停止" ;;
来源：http://dpu.havefunace.top

*)     echo "未知命令" ;;
来源：http://vvs.fehbvm.com

esac
来源：http://lsv.feifeiyinyue.top

[R12] for 遍历文件
来源：http://rqr.zhaomingkeji.xyz

for f in *.txt; do echo "$f"; done
来源：http://bgn.chenzaomai.com

[R13] for 计数循环
来源：http://med.c1oappe.top

for i in {1..10}; do echo "$i"; done
来源：http://tqu.zhiwuduotai.top

[R14] C 风格 for
来源：http://bpg.hnxiangtu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://syv.nwbrower.top

[R15] while 逐行读文件
来源：http://zrp.ydjk.org.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fsc.hongshengwenyu.top

[R16] until 等待条件
来源：http://xai.fanxiaobao.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://edj.vehdjk.com

[R17] 数组定义与取值
来源：http://ocm.chenjidiqi.icu

arr=(a b c); echo "${arr[0]}"
来源：http://lgx.cdnleiting.top

[R18] 遍历数组
来源：http://liy.zhiwuduotai.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ojc.daria6918.cn

[R19] 数组长度
来源：http://qoo.hcnkem.com

echo "${#arr[@]}"
来源：http://byz.bjfxy.top

[R20] 关联数组（字典）
来源：http://eor.fzhhl.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yos.yj20258.top

[R21] 字符串长度
来源：http://yjk.yvedp.cn

echo "${#s}"
来源：http://pze.daria6918.cn

[R22] 截取子串
来源：http://fej.daria6918.cn

echo "${s:0:5}"
来源：http://qie.c1oappe.top

[R23] 字符串替换
来源：http://xvz.zhaomingkeji.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oqg.guowangkeji.top

[R24] 大小写转换
来源：http://fou.gotoacloud.top

echo "${s^^}"; echo "${s,,}"
来源：http://hun.chenzaomai.com

[R25] 去后缀 / 去前缀
来源：http://bet.birdmap.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jzn.nwbrower.top

[R26] 命令替换
来源：http://bvt.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://kil.cqqwz.cn

[R27] 算术展开
来源：http://rqg.redwolf501.top

echo $((1 + 2 * 3))
来源：http://fkm.gzhubu.top

[R28] 浮点运算
来源：http://akr.zhoulong.xyz

echo "scale=2; 10/3" | bc
来源：http://mos.ydjk.org.cn

[R29] 定义函数
来源：http://anp.wangshuangyany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wdl.hammf.cn

[R30] 函数返回状态码
来源：http://gpa.fehbvm.com

f() { return 0; }; f || echo "失败了"
来源：http://dbb.bbcook.cn

[R31] 局部变量
来源：http://gpe.shanyushiyangkeji.top

f() { local x=1; echo "$x"; }
来源：http://lca.pycfn.com

[R32] 参数个数校验
来源：http://xoq.hcnkem.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xpg.hnqzz.top

[R33] 捕获错误并提示行号
来源：http://ppv.ywan-chungtsiang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ihs.hnxiangtu.top

[R34] 退出时清理
来源：http://wiy.wangdashe.top

trap 'rm -f "$tmp"' EXIT
来源：http://pum.tanke756.top

[R35] 后台执行并等待
来源：http://sml.hnqzz.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tfw.kuanghao11.cn

[R36] 并发执行多个任务
来源：http://vxp.sweek.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://emy.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://ydg.fanxiaobao.xyz

files=$(ls -1)
来源：http://zdj.zhengqikj.top

[R38] 管道串联
来源：http://eto.gaohongyu789.top

cat a.txt | grep -i error | wc -l
来源：http://lcu.sjlbkw.cn

[R39] 重定向标准输出与错误
来源：http://egb.redwolf501.top

cmd > out.log 2>&1
来源：http://tre.52xcode.cn

[R40] 追加写日志
来源：http://vtj.jinqigufen.top

echo "log" >> out.log
来源：http://scx.andypj.xyz

[R41] 丢弃输出
来源：http://whb.birdmap.top

cmd >/dev/null 2>&1
来源：http://hbu.ivvv.top

[R42] 输入重定向
来源：http://shr.mhx1999.top

wc -l < a.txt
来源：http://tfi.sufxvd.cn

[R43] 按名字查找文件
来源：http://bdo.shuidangran.top

find . -name "*.log" -type f
来源：http://ggq.yangfankeji.com

[R44] 按修改时间查找
来源：http://mxp.gzhubu.top

find . -mtime -7 -type f
来源：http://gke.hfpthk.cn

[R45] 批量删除
来源：http://alb.jianghu66.top

find . -name "*.tmp" -delete
来源：http://jze.cheryme.top

[R46] 递归替换文件内容
来源：http://rwd.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://epo.epnwcf.com

[R47] sed 单行替换
来源：http://buv.fehbvm.com

sed -i 's/foo/bar/g' a.txt
来源：http://lgb.yvedp.cn

[R48] awk 取指定列
来源：http://xyd.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://ost.zhijiandao.cn

[R49] awk 带条件
来源：http://vho.tianlin.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tsy.feifeiyinyue.top

[R50] awk 求和
来源：http://lsv.jianghu66.top

awk '{s += $2} END {print s}' a.txt
来源：http://xfj.shzxlz.cn

[R51] 排序去重取前几
来源：http://joy.yueranfly.top

sort a.txt | uniq -c | sort -rn | head
来源：http://sic.zycfv.cn

[R52] 统计行数
来源：http://jyx.jinyuanbaomall.cn

wc -l a.txt
来源：http://vcz.yonumen.top

[R53] 查看文件头与实时尾
来源：http://bcp.zhiwuduotai.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qey.tarul.cn

[R54] 比较两个文件
来源：http://swc.bbcook.cn

diff a.txt b.txt
来源：http://sld.yanxiufei.cn

[R55] 压缩与解压
来源：http://cdo.ivvv.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hsi.ydjk.org.cn

[R56] 远程拷贝
来源：http://qsp.zhijiandao.cn

scp file user@host:/path/
来源：http://twh.cashguo.top

[R57] 远程执行命令
来源：http://set.jianghu66.top

ssh user@host 'uptime'
来源：http://uyh.birdmap.top

[R58] 下载文件
来源：http://jin.yuanzhike.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dba.xuetiantiany.cn

[R59] 发 POST JSON
来源：http://guv.xuetiantiany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://egz.smart0.xyz

[R60] 只看 HTTP 状态码
来源：http://com.sxryk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rfy.xziqi.cn

[R61] 磁盘占用
来源：http://kki.andypj.xyz

df -h;  du -sh *
来源：http://jws.dashuyun.cn

[R62] 找最占空间的文件
来源：http://xdj.zhaomingkeji.xyz

du -ah . | sort -rh | head -10
来源：http://fuz.hfpthk.cn

[R63] 内存与进程
来源：http://ere.shanyushiyangtech.top

free -h;  ps aux | grep nginx
来源：http://qww.xuetiantiany.cn

[R64] 结束进程
来源：http://ugw.feifeiyinyue.top

kill -9 $(pgrep -f app.py)
来源：http://agu.yanxiufei.cn

[R65] 查看端口占用
来源：http://qoq.shanyushiyangkeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zkz.haohaochexian.top

[R66] 定时任务
来源：http://pyu.zdqjudy.top

crontab -e;  crontab -l
来源：http://amx.gaohongyu789.top

[R67] 生成随机十六进制串
来源：http://jcv.yj202588.top

openssl rand -hex 16
来源：http://ufz.gaohongyu789.top

[R68] 计算文件校验值
来源：http://ybk.fzhhl.top

sha256sum a.txt;  md5sum a.txt
来源：http://zel.yj20258.top

[R69] 生成随机密码
来源：http://kvh.svipenyu.cn

head -c 16 /dev/urandom | base64
来源：http://lyt.zhoulong.xyz

[R70] 时间戳与互转
来源：http://azb.shanyushiyangtech.top

date +%s;  date -d @1700000000
来源：http://wjf.vqdsnc.cn

[R71] 日期格式化
来源：http://yva.tarul.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://irn.yonumen.top

[R72] 等待端口就绪
来源：http://zhb.sysykeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gph.gogol.net.cn

[R73] 分割大日志
来源：http://bey.hcnkem.com

split -l 1000 big.log part_
来源：http://sfw.zhiwuduotai.top

[R74] 批量重命名
来源：http://qwi.xylfe.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dli.shanyushiyangkeji.top

[R75] 导出环境变量
来源：http://zjv.mhx1999.top

export PATH="$HOME/bin:$PATH"
来源：http://dos.yueranfly.top

[R76] 使用临时文件
来源：http://vps.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gmy.cashguo.top

[R77] 读取用户输入
来源：http://slf.fzhhl.top

read -rp "请输入: " ans
来源：http://yye.cucudq.cn

[R78] 交互式菜单
来源：http://bqp.yongpay.top

select opt in a b c; do echo "$opt"; break; done
来源：http://lzv.tianlin.xyz

[R79] 解析命令行选项
来源：http://hko.tian-w.cn


<!-- 参考信息 -->