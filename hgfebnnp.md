代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kcx.havefunace.top

[Q40] 交叉连接（笛卡尔积）
来源：http://kgt.kuanghao11.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://akk.quarkkingdee.top

[Q41] 多表连接
来源：http://wrr.yanxiufei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yuu.jinghuilouyu.cn

JOIN users u ON u.id = o.user_id
来源：http://jnz.yangfankeji.com

JOIN products p ON p.id = o.product_id;
来源：http://iov.zhoulong.xyz

[Q42] 连接条件附加过滤
来源：http://caq.ehwqpu.com

SELECT u.name, o.amount FROM users u
来源：http://xnm.jqgufenzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cbo.aizwys.cn

[Q43] 标量子查询
来源：http://orv.feifeiyinyue.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hmv.hnqzz.top

[Q44] IN 子查询
来源：http://gtu.c1oappe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://klf.hywenlv.cn

[Q45] EXISTS 判断存在
来源：http://nyy.hysaishi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://efe.cashguo.top

[Q46] NOT EXISTS 判断不存在
来源：http://vjx.pengpengdd.cyou

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ghs.52xcode.cn

[Q47] 与平均值比较
来源：http://ezm.dashuyun.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sul.iojbl.cn

[Q48] CTE 公用表表达式
来源：http://tfc.jianghu66.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lgf.zhengqikj.top

SELECT * FROM t WHERE c > 5;
来源：http://hlh.yanxiufei.cn

[Q49] 更新单行
来源：http://qgo.nwbrower.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ywg.epnwcf.com

[Q50] 批量更新
来源：http://ubu.guannengcc.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vdo.ctjpmb.com

[Q51] 用子查询更新
来源：http://sfw.daxiang520.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://atm.sweek.top

[Q52] 删除指定行
来源：http://dsh.vqdsnc.cn

DELETE FROM users WHERE id = 10;
来源：http://cvh.hnqzz.top

[Q53] 按条件删除
来源：http://tmb.xylfe.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lax.jinqigufen.top

[Q54] 清空表
来源：http://vmb.daria6918.cn

TRUNCATE TABLE logs;
来源：http://ycf.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://rza.jiagoushi.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://djk.jyoumei.cn

[Q56] 密集排名（并列不占位）
来源：http://pks.gaohongyu789.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cnd.xuanzx.com

[Q57] 行号
来源：http://yba.xinyue.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ktn.bbcook.cn

[Q58] 累计求和
来源：http://qko.sufxvd.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vzo.vehdjk.com

[Q59] 分组内累计
来源：http://kdf.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kid.ppjwa.cn

[Q60] 取上一行 / 下一行
来源：http://wtn.daria6918.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://twb.zhongyouzk.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qiz.ydzc1.top

[Q61] 移动平均
来源：http://sld.ivvv.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nhw.hcnkem.com

[Q62] 分组占比
来源：http://lbp.fzhhl.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zdw.hysaishi.cn

[Q63] 开启事务
来源：http://opw.uphjek.com

START TRANSACTION;                -- 或 BEGIN
来源：http://prs.wangdashe.top

[Q64] 提交事务
来源：http://mkh.fzhhl.top

COMMIT;
来源：http://dtz.svipenyu.cn

[Q65] 回滚事务
来源：http://xho.gzhubu.top

ROLLBACK;
来源：http://ofz.jiagoushi.top

[Q66] 行锁查询
来源：http://jah.svipenyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oaq.uphjek.com

[Q67] 设置隔离级别
来源：http://juk.guannengcc.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://evy.gaohongyu789.top

[Q68] 保存点
来源：http://wuh.daria6918.cn

SAVEPOINT sp1;
来源：http://ske.yangfankeji.com

ROLLBACK TO sp1;
来源：http://sri.epnwcf.com

[Q69] 查看执行计划
来源：http://utg.hfpthk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kda.ybcxt.top

[Q70] 更新统计信息
来源：http://kcl.tianlin.xyz

ANALYZE TABLE users;
来源：http://jle.smart0.xyz

[Q71] 查看建表语句
来源：http://ngy.svipenyu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yxe.cheryme.top

[Q72] 查看索引
来源：http://pik.zhixingplan.top

SHOW INDEX FROM users;
来源：http://wfi.zhoulong.xyz

[Q73] 查看表状态
来源：http://sbt.jlsjyb.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dmm.shangyingyoupin.top

[Q74] 强制使用索引
来源：http://eed.nanxinkj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wjf.yuanzhike.top

[Q75] 日期格式化
来源：http://kbw.jqgfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jbo.ehwqpu.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://otn.gotoacloud.top

[Q76] 按天统计
来源：http://rrp.chenjidiqi.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zhi.c1oappe.top

[Q77] 时间加减
来源：http://nhk.hammf.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hgz.kuanghao11.cn

[Q78] 当前时间
来源：http://ddi.9152youxi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ttc.yanxiufei.cn

[Q79] 字符串拼接
来源：http://mos.smart0.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://eub.redwolf501.top

[Q80] 字符串截取
来源：http://vdr.jiagoushi.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dap.dashuyun.cn

[Q81] 字符串替换
来源：http://mqe.xuanzx.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ahg.nwbrower.top

[Q82] 字符长度与字节长度
来源：http://fdu.chenjidiqi.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eqv.guannengcc.top

[Q83] 大小写转换
来源：http://orp.nanxinkj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bzb.epnwcf.com

[Q84] 去除首尾空格
来源：http://hoh.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://ofl.jlsjyb.cn

[Q85] 数值取整
来源：http://rgn.ybcxt.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gyh.zdbjq.cn

[Q86] 读取 JSON 字段
来源：http://pdv.svipenyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rqh.0kj1m.cn

[Q87] JSON 字段做条件
来源：http://tuh.wangshuangyany.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kje.yuxming.cn

[Q88] 行转列（条件聚合）
来源：http://rmn.cdnleiting.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xwm.epnwcf.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qkg.fzhhl.top

[Q89] 判断表是否存在
来源：http://ebw.guannengcc.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dvx.vqdsnc.cn

[Q90] 生成序号列
来源：http://bji.cucudq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eww.sysykeji.top

================================================================================
来源：http://ofj.nwbrower.top

R. Bash 专题
来源：http://dan.daria6918.cn

================================================================================
来源：http://kxm.zhaomingkeji.xyz

[R01] shebang 与严格模式
来源：http://gcf.mhx1999.top

#!/usr/bin/env bash
来源：http://mbf.jinghuilouyu.cn

set -euo pipefail
来源：http://wgr.sjlbkw.cn

[R02] 变量赋值与使用
来源：http://pkj.ehwqpu.com

name="Tom"; echo "$name"
来源：http://ewj.zdqjudy.top

[R03] 只读变量
来源：http://bnc.jianghu66.top

readonly PI=3.14
来源：http://drm.shanyushiyangtech.top

[R04] 位置参数
来源：http://etb.haohaochexian.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oyr.vehdjk.com

[R05] 参数默认值
来源：http://axn.wangdashe.top

name="${1:-default}"
来源：http://ksz.sysykeji.top

[R06] 判断命令是否存在
来源：http://ljr.gaohongyu789.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cgo.ybcxt.top

[R07] if 判断文件
来源：http://otn.snrcjt.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uxh.xingfuxueyuan.xyz

[R08] 数值比较
来源：http://kzc.hesvh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wvd.fktsv.cn

[R09] 字符串比较
来源：http://uon.jqgufenzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tjg.ydjk.org.cn

[R10] 正则匹配
来源：http://gdg.andypj.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wqt.vehdjk.com

[R11] case 多分支
来源：http://bkn.jqgfzy.top

case "$1" in
来源：http://wbw.quarkkingdee.top

start) echo "启动" ;;
来源：http://uxw.yonumen.top

stop)  echo "停止" ;;
来源：http://vzy.jqgfzy.top

*)     echo "未知命令" ;;
来源：http://jki.shuidangran.top

esac
来源：http://ybl.snrcjt.cn

[R12] for 遍历文件
来源：http://rdn.yj202588.top

for f in *.txt; do echo "$f"; done
来源：http://dvm.jinghuilouyu.cn

[R13] for 计数循环
来源：http://etn.jinyuanbaomall.cn

for i in {1..10}; do echo "$i"; done
来源：http://kru.hnqzz.top

[R14] C 风格 for
来源：http://iya.fengsongda.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hip.jinqigfzy.top

[R15] while 逐行读文件
来源：http://hhg.jqgufenzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vpa.yvedp.cn

[R16] until 等待条件
来源：http://jvb.jianghu66.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vch.feifeiyinyue.top

[R17] 数组定义与取值
来源：http://kbw.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ass.sweek.top

[R18] 遍历数组
来源：http://hbi.nanxinkj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zuk.xinyue.icu

[R19] 数组长度
来源：http://pco.havefunace.top

echo "${#arr[@]}"
来源：http://yll.cashguo.top

[R20] 关联数组（字典）
来源：http://dbb.meibo888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fjd.hesvh.cn

[R21] 字符串长度
来源：http://otx.yvedp.cn

echo "${#s}"
来源：http://mib.shuidangran.top

[R22] 截取子串
来源：http://swh.yj20258888.top

echo "${s:0:5}"
来源：http://sgf.jinqigfzy.top

[R23] 字符串替换
来源：http://tqy.hnxiangtu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lpg.zhixingplan.top

[R24] 大小写转换
来源：http://tbv.jinyuanbaomall.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jsh.yuxming.cn

[R25] 去后缀 / 去前缀
来源：http://oyx.bjfxy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qvb.hcnkem.com

[R26] 命令替换
来源：http://ghm.fktsv.cn

now=$(date +%F); echo "$now"
来源：http://tub.haohaochexian.top

[R27] 算术展开
来源：http://xiv.jlsjyb.cn

echo $((1 + 2 * 3))
来源：http://quc.feifeiyinyue.top

[R28] 浮点运算
来源：http://qir.fehbvm.com

echo "scale=2; 10/3" | bc
来源：http://msw.zycfv.cn

[R29] 定义函数
来源：http://gwv.zdqjudy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vkf.xuanzx.com

[R30] 函数返回状态码
来源：http://mjn.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://yew.sysykeji.top

[R31] 局部变量
来源：http://xaa.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://vqk.hnxiangtu.top

[R32] 参数个数校验
来源：http://fio.jinyuanbaomall.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tmu.epnwcf.com

[R33] 捕获错误并提示行号
来源：http://crj.wangshuangyany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://idk.jinqigfzy.top

[R34] 退出时清理
来源：http://kbq.snrcjt.cn

trap 'rm -f "$tmp"' EXIT
来源：http://scd.cheryme.top

[R35] 后台执行并等待
来源：http://evd.yuxming.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uyn.hesvh.cn

[R36] 并发执行多个任务
来源：http://xny.yfazqb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ugd.gogol.net.cn

[R37] 把输出赋给变量
来源：http://cvg.zhijiandao.cn

files=$(ls -1)
来源：http://hig.bbcook.cn

[R38] 管道串联
来源：http://shz.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://pyd.andypj.xyz

[R39] 重定向标准输出与错误
来源：http://atp.yuanzhike.top

cmd > out.log 2>&1
来源：http://cap.redwolf501.top

[R40] 追加写日志
来源：http://ylt.zhaomingkeji.xyz

echo "log" >> out.log
来源：http://zgb.cashguo.top

[R41] 丢弃输出
来源：http://yci.jyoumei.cn

cmd >/dev/null 2>&1
来源：http://baw.jqgfzy.top

[R42] 输入重定向
来源：http://dzb.yvedp.cn

wc -l < a.txt
来源：http://yso.fengsongda.top

[R43] 按名字查找文件
来源：http://fkd.xuanzx.com

find . -name "*.log" -type f
来源：http://pvs.daxiang520.top

[R44] 按修改时间查找
来源：http://adw.jinqigufen.top

find . -mtime -7 -type f
来源：http://czp.hesvh.cn

[R45] 批量删除
来源：http://kpg.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://yql.fanxiaobao.xyz

[R46] 递归替换文件内容
来源：http://onp.zhixingplan.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mma.ctjpmb.com

[R47] sed 单行替换
来源：http://gmr.svipenyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vme.ivvv.top

[R48] awk 取指定列
来源：http://vdz.hammf.cn

awk '{print $1, $3}' a.txt
来源：http://lov.aizwys.cn

[R49] awk 带条件
来源：http://mod.shuidangran.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hqd.yangfankeji.com

[R50] awk 求和
来源：http://yis.bbcook.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xuv.gotoacloud.top

[R51] 排序去重取前几
来源：http://xdg.sxryk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mew.zhaomingkeji.xyz

[R52] 统计行数
来源：http://xrm.zhoulong.xyz

wc -l a.txt
来源：http://xcd.kuanghao11.cn

[R53] 查看文件头与实时尾
来源：http://bmg.tianlin.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ccc.kuanghao11.cn

[R54] 比较两个文件
来源：http://cmd.cheryme.top

diff a.txt b.txt
来源：http://hsc.yongpay.top

[R55] 压缩与解压
来源：http://qyw.hammf.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hju.guannengcc.top

[R56] 远程拷贝
来源：http://dtu.svipenyu.cn

scp file user@host:/path/
来源：http://tjs.yj20258.top

[R57] 远程执行命令
来源：http://bfk.shuidangran.top

ssh user@host 'uptime'
来源：http://yip.jqgufenzy.top

[R58] 下载文件
来源：http://mra.jlsjyb.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aga.nwbrower.top

[R59] 发 POST JSON
来源：http://qra.sysykeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vfl.chenzaomai.com

[R60] 只看 HTTP 状态码
来源：http://guz.zhengqikj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gxa.ivvv.top

[R61] 磁盘占用
来源：http://kmh.0kj1m.cn

df -h;  du -sh *
来源：http://owq.zhixingplan.top

[R62] 找最占空间的文件
来源：http://grk.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://ktb.snrcjt.cn

[R63] 内存与进程
来源：http://pot.wangdashe.top

free -h;  ps aux | grep nginx
来源：http://wcv.zycfv.cn

[R64] 结束进程
来源：http://bls.cdnleiting.top

kill -9 $(pgrep -f app.py)
来源：http://zar.xinyue.icu

[R65] 查看端口占用
来源：http://kon.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wjz.chenzaomai.com

[R66] 定时任务
来源：http://kji.zhongyouzk.top

crontab -e;  crontab -l
来源：http://mmn.haohaochexian.top

[R67] 生成随机十六进制串
来源：http://trl.wangshuangyany.cn

openssl rand -hex 16
来源：http://qnx.sweek.top

[R68] 计算文件校验值
来源：http://spt.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://psa.quarkkingdee.top

[R69] 生成随机密码
来源：http://pju.xingfuxueyuan.xyz

head -c 16 /dev/urandom | base64
来源：http://qye.jiagoushi.top

[R70] 时间戳与互转
来源：http://vap.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://psf.52xcode.cn

[R71] 日期格式化
来源：http://kbb.quarkkingdee.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rvg.vqdsnc.cn

[R72] 等待端口就绪
来源：http://eog.andypj.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://ifg.wangdashe.top

[R73] 分割大日志
来源：http://afj.hongshengwenyu.top

split -l 1000 big.log part_
来源：http://eot.zycfv.cn

[R74] 批量重命名
来源：http://ggl.ydzc1.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ree.dashuyun.cn

[R75] 导出环境变量
来源：http://ttb.kuanghao11.cn

export PATH="$HOME/bin:$PATH"
来源：http://ujs.fengsongda.top

[R76] 使用临时文件
来源：http://vpi.redwolf501.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ahw.cdnleiting.top

[R77] 读取用户输入
来源：http://pvg.ydjk.org.cn

read -rp "请输入: " ans
来源：http://rwm.zhijiandao.cn

[R78] 交互式菜单
来源：http://izv.guannengcc.top

select opt in a b c; do echo "$opt"; break; done
来源：http://eit.jinqigfzy.top

[R79] 解析命令行选项
来源：http://uke.yanxiufei.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://knz.wangshuangyany.cn

[R80] 查看脚本执行耗时
来源：http://ebk.ppjwa.cn

time ./run.sh
来源：http://gwg.gogol.net.cn

================================================================================
来源：http://uqy.52xcode.cn

S. C / C++ 专题
来源：http://zvi.chenzaomai.com

================================================================================
来源：http://hfp.aibaodan.cn

[S01] C：Hello World
来源：http://qsh.zhongyouzk.top

#include <stdio.h>
来源：http://hnd.fengsongda.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://huz.cashguo.top

[S02] C：变量与格式化输出
来源：http://bjx.xylfe.cn

int a = 10; printf("%d\n", a);
来源：http://cbl.pycfn.com

[S03] C：读入整数
来源：http://crc.yuanzhike.top

int x; scanf("%d", &x);
来源：http://ppn.fzhhl.top

[S04] C：字符串复制
来源：http://fva.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pca.hnqzz.top

[S05] C：字符串长度
来源：http://qmo.nanxinkj.top

strlen(s)
来源：http://vaf.52xcode.cn

[S06] C：字符串比较
来源：http://viz.gzhubu.top

strcmp(a, b) == 0
来源：http://mha.yuanzhike.top

[S07] C：数组遍历求和
来源：http://hgb.cqqwz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://aaz.vqdsnc.cn

[S08] C：动态内存分配与释放
来源：http://lnq.hysaishi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wgc.c1oappe.top

[S09] C：结构体定义与初始化
来源：http://lkx.zdqjudy.top


<!-- 参考信息 -->