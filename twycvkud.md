代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://gsf.zycfv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fec.0kj1m.cn

[Q39] 自连接（查上下级）
来源：http://dwk.zhaomingkeji.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://cml.nwbrower.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qpg.sufxvd.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nrd.jianghu66.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lft.xylfe.cn

[Q41] 多表连接
来源：http://flg.guannengcc.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pav.yanxiufei.cn

JOIN users u ON u.id = o.user_id
来源：http://ouj.fengsongda.top

JOIN products p ON p.id = o.product_id;
来源：http://cdd.gotoacloud.top

[Q42] 连接条件附加过滤
来源：http://bho.jiagoushi.top

SELECT u.name, o.amount FROM users u
来源：http://xiu.bbcook.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ngh.jlsjyb.cn

[Q43] 标量子查询
来源：http://qgs.bbcook.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://upy.pycfn.com

[Q44] IN 子查询
来源：http://gjz.epnwcf.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ogn.hesvh.cn

[Q45] EXISTS 判断存在
来源：http://fzx.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vtn.iojbl.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xme.fengsongda.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rsi.ctjpmb.com

[Q47] 与平均值比较
来源：http://wpt.aizwys.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jyn.sysykeji.top

[Q48] CTE 公用表表达式
来源：http://uqy.aibaodan.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ptx.yueranfly.top

SELECT * FROM t WHERE c > 5;
来源：http://vjy.xuanzx.com

[Q49] 更新单行
来源：http://ydu.hammf.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zoj.zdqjudy.top

[Q50] 批量更新
来源：http://zcd.yj20258888.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nxh.gogol.net.cn

[Q51] 用子查询更新
来源：http://fij.xingfuxueyuan.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pim.redwolf501.top

[Q52] 删除指定行
来源：http://hdf.316326.xyz

DELETE FROM users WHERE id = 10;
来源：http://hgg.hfpthk.cn

[Q53] 按条件删除
来源：http://zhu.zhijiandao.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xwa.zhaomingkeji.xyz

[Q54] 清空表
来源：http://goz.zdqjudy.top

TRUNCATE TABLE logs;
来源：http://gon.redwolf501.top

[Q55] 排名（并列占位）
来源：http://abm.iojbl.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ali.birdmap.top

[Q56] 密集排名（并列不占位）
来源：http://tqn.zhongyouzk.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://brs.yj20258888.top

[Q57] 行号
来源：http://iez.guowangkeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pyh.bbcook.cn

[Q58] 累计求和
来源：http://dvy.gaohongyu789.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hgi.hnqzz.top

[Q59] 分组内累计
来源：http://gtn.shzxlz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://iec.zhaomingkeji.xyz

[Q60] 取上一行 / 下一行
来源：http://kcz.316326.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://twd.pycfn.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dvo.52xcode.cn

[Q61] 移动平均
来源：http://hhl.ctjpmb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oiw.pycfn.com

[Q62] 分组占比
来源：http://rly.tian-w.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gss.xingfuxueyuan.xyz

[Q63] 开启事务
来源：http://bdu.zhixingplan.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dan.jyoumei.cn

[Q64] 提交事务
来源：http://dxf.nanxinkj.top

COMMIT;
来源：http://gks.aibaodan.cn

[Q65] 回滚事务
来源：http://tqe.smart0.xyz

ROLLBACK;
来源：http://npa.nanxuanxn.top

[Q66] 行锁查询
来源：http://pyx.xuetiantiany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xtn.xylfe.cn

[Q67] 设置隔离级别
来源：http://vss.daxiang520.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fvb.zycfv.cn

[Q68] 保存点
来源：http://gtx.tanke756.top

SAVEPOINT sp1;
来源：http://tpj.ydzc1.top

ROLLBACK TO sp1;
来源：http://fzx.daxiang520.top

[Q69] 查看执行计划
来源：http://mtn.ywan-chungtsiang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zjs.shangyingyoupin.top

[Q70] 更新统计信息
来源：http://qme.xuanzx.com

ANALYZE TABLE users;
来源：http://ypb.bbcook.cn

[Q71] 查看建表语句
来源：http://yyb.bbcook.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ecs.ydzc1.top

[Q72] 查看索引
来源：http://biq.snrcjt.cn

SHOW INDEX FROM users;
来源：http://txo.shangyingyoupin.top

[Q73] 查看表状态
来源：http://qjn.yanxiufei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://sel.fengsongda.top

[Q74] 强制使用索引
来源：http://pht.cashguo.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://axv.fehbvm.com

[Q75] 日期格式化
来源：http://rvy.xinyue.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yby.gaohongyu789.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uwn.hcnkem.com

[Q76] 按天统计
来源：http://zrd.sjlbkw.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://npq.daria6918.cn

[Q77] 时间加减
来源：http://lbu.sysykeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cby.zhongyouzk.top

[Q78] 当前时间
来源：http://ytx.sufxvd.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aty.uphjek.com

[Q79] 字符串拼接
来源：http://akd.0kj1m.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://olp.feifeiyinyue.top

[Q80] 字符串截取
来源：http://vem.yfazqb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zmd.zhijiandao.cn

[Q81] 字符串替换
来源：http://yya.aibaodan.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rkz.ppjwa.cn

[Q82] 字符长度与字节长度
来源：http://egi.yuxming.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vom.aizwys.cn

[Q83] 大小写转换
来源：http://ysa.fanxiaobao.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://adq.ehwqpu.com

[Q84] 去除首尾空格
来源：http://riy.snrcjt.cn

SELECT TRIM(name) FROM users;
来源：http://twv.shzxlz.cn

[Q85] 数值取整
来源：http://rxd.chenzaomai.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ikk.ywan-chungtsiang.top

[Q86] 读取 JSON 字段
来源：http://ymj.jinghuilouyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bjr.yvedp.cn

[Q87] JSON 字段做条件
来源：http://wsx.hfpthk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cvx.yvedp.cn

[Q88] 行转列（条件聚合）
来源：http://wav.fanxiaobao.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hkw.hcnkem.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xbj.ybcxt.top

[Q89] 判断表是否存在
来源：http://yly.zhaomingkeji.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qve.iojbl.cn

[Q90] 生成序号列
来源：http://xpn.fehbvm.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lzh.sxryk.cn

================================================================================
来源：http://nfo.ybcxt.top

R. Bash 专题
来源：http://vom.iojbl.cn

================================================================================
来源：http://kiq.ppjwa.cn

[R01] shebang 与严格模式
来源：http://tms.pycfn.com

#!/usr/bin/env bash
来源：http://ttl.hnqzz.top

set -euo pipefail
来源：http://xhb.hnxiangtu.top

[R02] 变量赋值与使用
来源：http://eus.fzhhl.top

name="Tom"; echo "$name"
来源：http://ttt.fzhhl.top

[R03] 只读变量
来源：http://qlm.birdmap.top

readonly PI=3.14
来源：http://nop.jinyuanbaomall.cn

[R04] 位置参数
来源：http://kae.shanyushiyangtech.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gtr.tanke756.top

[R05] 参数默认值
来源：http://mub.yangfankeji.com

name="${1:-default}"
来源：http://vxj.daria6918.cn

[R06] 判断命令是否存在
来源：http://gir.bbcook.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://whr.epnwcf.com

[R07] if 判断文件
来源：http://qey.redwolf501.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zqi.meibo888.top

[R08] 数值比较
来源：http://hlb.nwbrower.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gbd.chenlongwang.top

[R09] 字符串比较
来源：http://qay.chenlongwang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dmc.epnwcf.com

[R10] 正则匹配
来源：http://ngs.gotoacloud.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hqr.andypj.xyz

[R11] case 多分支
来源：http://qvx.pengpengdd.cyou

case "$1" in
来源：http://ggf.aizwys.cn

start) echo "启动" ;;
来源：http://xbr.cdnleiting.top

stop)  echo "停止" ;;
来源：http://whw.yueranfly.top

*)     echo "未知命令" ;;
来源：http://gbx.hywenlv.cn

esac
来源：http://yvs.haohaochexian.top

[R12] for 遍历文件
来源：http://vou.chenzaomai.com

for f in *.txt; do echo "$f"; done
来源：http://oaa.daria6918.cn

[R13] for 计数循环
来源：http://ajf.jlsjyb.cn

for i in {1..10}; do echo "$i"; done
来源：http://pnc.ydjk.org.cn

[R14] C 风格 for
来源：http://cbu.aizwys.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sbs.yanxiufei.cn

[R15] while 逐行读文件
来源：http://oil.zdbjq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://elm.yangfankeji.com

[R16] until 等待条件
来源：http://tid.c1oappe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://run.tian-w.cn

[R17] 数组定义与取值
来源：http://qqb.dashuyun.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gbi.jianghu66.top

[R18] 遍历数组
来源：http://qdx.vehdjk.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pmx.chenlongwang.top

[R19] 数组长度
来源：http://txv.aibaodan.cn

echo "${#arr[@]}"
来源：http://lcv.hysaishi.cn

[R20] 关联数组（字典）
来源：http://ost.nwbrower.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nex.hongshengwenyu.top

[R21] 字符串长度
来源：http://hqy.zdbjq.cn

echo "${#s}"
来源：http://rug.meibo888.top

[R22] 截取子串
来源：http://vqi.xuetiantiany.cn

echo "${s:0:5}"
来源：http://smp.xuetiantiany.cn

[R23] 字符串替换
来源：http://sii.tianlin.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wdk.sufxvd.cn

[R24] 大小写转换
来源：http://atl.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yyk.ivvv.top

[R25] 去后缀 / 去前缀
来源：http://szz.xylfe.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vpq.zdbjq.cn

[R26] 命令替换
来源：http://iwn.hnqzz.top

now=$(date +%F); echo "$now"
来源：http://alr.cdnleiting.top

[R27] 算术展开
来源：http://xqu.xingfuxueyuan.xyz

echo $((1 + 2 * 3))
来源：http://dqw.jqgufenzy.top

[R28] 浮点运算
来源：http://mlr.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://kfi.ywan-chungtsiang.top

[R29] 定义函数
来源：http://ehn.vehdjk.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wgi.quarkkingdee.top

[R30] 函数返回状态码
来源：http://nkq.havefunace.top

f() { return 0; }; f || echo "失败了"
来源：http://lrs.snrcjt.cn

[R31] 局部变量
来源：http://ywl.cheryme.top

f() { local x=1; echo "$x"; }
来源：http://ozr.yongpay.top

[R32] 参数个数校验
来源：http://per.daxiang520.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yir.gogol.net.cn

[R33] 捕获错误并提示行号
来源：http://dfh.0kj1m.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://giz.jinqigfzy.top

[R34] 退出时清理
来源：http://nvg.ivvv.top

trap 'rm -f "$tmp"' EXIT
来源：http://idb.yvedp.cn

[R35] 后台执行并等待
来源：http://yxi.fengsongda.top

sleep 5 & pid=$!; wait "$pid"
来源：http://brs.yfazqb.com

[R36] 并发执行多个任务
来源：http://cwq.andypj.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wqi.yj20258.top

[R37] 把输出赋给变量
来源：http://hwo.shangyingyoupin.top

files=$(ls -1)
来源：http://gqw.pycfn.com

[R38] 管道串联
来源：http://ixk.yj20258.top

cat a.txt | grep -i error | wc -l
来源：http://tza.dianchejie.cn

[R39] 重定向标准输出与错误
来源：http://alu.kuanghao11.cn

cmd > out.log 2>&1
来源：http://okx.tarul.cn

[R40] 追加写日志
来源：http://tzv.yj20258.top

echo "log" >> out.log
来源：http://txs.hfpthk.cn

[R41] 丢弃输出
来源：http://ceg.zycfv.cn

cmd >/dev/null 2>&1
来源：http://zqz.hnxiangtu.top

[R42] 输入重定向
来源：http://ntj.chenjidiqi.icu

wc -l < a.txt
来源：http://nnk.haohaochexian.top

[R43] 按名字查找文件
来源：http://xvq.jiagoushi.top

find . -name "*.log" -type f
来源：http://bgz.gzhubu.top

[R44] 按修改时间查找
来源：http://mok.cdnleiting.top

find . -mtime -7 -type f
来源：http://cqs.sjlbkw.cn

[R45] 批量删除
来源：http://xlx.fengsongda.top

find . -name "*.tmp" -delete
来源：http://arz.redwolf501.top

[R46] 递归替换文件内容
来源：http://qdk.yj20258.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xah.chenzaomai.com

[R47] sed 单行替换
来源：http://pbr.wangshuangyany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://whg.guannengcc.top

[R48] awk 取指定列
来源：http://eru.hesvh.cn

awk '{print $1, $3}' a.txt
来源：http://dbj.jianghu66.top

[R49] awk 带条件
来源：http://dul.hongshengwenyu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mht.cdnleiting.top

[R50] awk 求和
来源：http://sql.zhiwuduotai.top

awk '{s += $2} END {print s}' a.txt
来源：http://ylm.yj202588.top

[R51] 排序去重取前几
来源：http://hbv.daxiang520.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jvs.vehdjk.com

[R52] 统计行数
来源：http://ftz.cashguo.top

wc -l a.txt
来源：http://ngc.yueranfly.top

[R53] 查看文件头与实时尾
来源：http://gcb.yueranfly.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kiu.kuanghao11.cn

[R54] 比较两个文件
来源：http://pyq.yj202588.top

diff a.txt b.txt
来源：http://ukj.tian-w.cn

[R55] 压缩与解压
来源：http://wap.cdnleiting.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ytp.svipenyu.cn

[R56] 远程拷贝
来源：http://duo.yvedp.cn

scp file user@host:/path/
来源：http://scd.yfazqb.com

[R57] 远程执行命令
来源：http://bxl.zycfv.cn

ssh user@host 'uptime'
来源：http://fyd.dianchejie.cn

[R58] 下载文件
来源：http://qgk.hysaishi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rdi.fengsongda.top

[R59] 发 POST JSON
来源：http://cdy.ehwqpu.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lnp.cashguo.top

[R60] 只看 HTTP 状态码
来源：http://saq.ivvv.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://amp.gzhubu.top

[R61] 磁盘占用
来源：http://hno.52xcode.cn

df -h;  du -sh *
来源：http://cna.meibo888.top

[R62] 找最占空间的文件
来源：http://ddv.sxryk.cn

du -ah . | sort -rh | head -10
来源：http://qiw.havefunace.top

[R63] 内存与进程
来源：http://idu.gaohongyu789.top

free -h;  ps aux | grep nginx
来源：http://tkf.aibaodan.cn

[R64] 结束进程
来源：http://gak.kuanghao11.cn

kill -9 $(pgrep -f app.py)
来源：http://xsu.hysaishi.cn

[R65] 查看端口占用
来源：http://svd.epnwcf.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pef.gotoacloud.top

[R66] 定时任务
来源：http://yyz.svipenyu.cn

crontab -e;  crontab -l
来源：http://oyo.xuetiantiany.cn

[R67] 生成随机十六进制串
来源：http://zjk.316326.xyz

openssl rand -hex 16
来源：http://guf.xziqi.cn

[R68] 计算文件校验值
来源：http://oli.xingfuxueyuan.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://kuz.jyoumei.cn

[R69] 生成随机密码
来源：http://afd.bjfxy.top

head -c 16 /dev/urandom | base64
来源：http://myp.cdnleiting.top

[R70] 时间戳与互转
来源：http://zzc.jianghu66.top

date +%s;  date -d @1700000000
来源：http://kpo.shuidangran.top

[R71] 日期格式化
来源：http://ecu.fehbvm.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://lfy.hnqzz.top

[R72] 等待端口就绪
来源：http://fxf.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wut.jinghuilouyu.cn

[R73] 分割大日志
来源：http://nnh.wangdashe.top

split -l 1000 big.log part_
来源：http://zxs.ppjwa.cn

[R74] 批量重命名
来源：http://wqx.gogol.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://syr.jiagoushi.top

[R75] 导出环境变量
来源：http://huu.hywenlv.cn

export PATH="$HOME/bin:$PATH"
来源：http://zry.guowangkeji.top

[R76] 使用临时文件
来源：http://rlf.haohaochexian.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wjb.cashguo.top

[R77] 读取用户输入
来源：http://cnj.zdbjq.cn

read -rp "请输入: " ans
来源：http://dxf.tanke756.top

[R78] 交互式菜单
来源：http://miw.yj202588.top

select opt in a b c; do echo "$opt"; break; done
来源：http://lbt.pycfn.com

[R79] 解析命令行选项
来源：http://vrh.yonumen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://atv.daria6918.cn

[R80] 查看脚本执行耗时
来源：http://bsh.shuidangran.top

time ./run.sh
来源：http://kbq.tanke756.top

================================================================================
来源：http://zak.gotoacloud.top

S. C / C++ 专题
来源：http://tzl.hnxiangtu.top

================================================================================
来源：http://ncd.zhoulong.xyz

[S01] C：Hello World
来源：http://rrr.tarul.cn

#include <stdio.h>
来源：http://uen.9152youxi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kkt.cdnleiting.top

[S02] C：变量与格式化输出
来源：http://zqg.yj20258888.top

int a = 10; printf("%d\n", a);
来源：http://zsn.hysaishi.cn

[S03] C：读入整数
来源：http://hpv.yonumen.top

int x; scanf("%d", &x);
来源：http://ipm.cheryme.top

[S04] C：字符串复制
来源：http://ogm.fanxiaobao.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://zig.birdmap.top

[S05] C：字符串长度
来源：http://xkb.aibaodan.cn

strlen(s)
来源：http://jgv.sysykeji.top

[S06] C：字符串比较
来源：http://lgd.gogol.net.cn

strcmp(a, b) == 0
来源：http://hmt.yanxiufei.cn

[S07] C：数组遍历求和
来源：http://sxv.birdmap.top


<!-- 参考信息 -->