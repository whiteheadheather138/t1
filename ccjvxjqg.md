代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://fgu.fanxiaobao.xyz

JOIN users u ON u.id = o.user_id
来源：http://pao.shanyushiyangtech.top

JOIN products p ON p.id = o.product_id;
来源：http://owf.zhongyouzk.top

[Q42] 连接条件附加过滤
来源：http://ebv.nwbrower.top

SELECT u.name, o.amount FROM users u
来源：http://odn.pengpengdd.cyou

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yta.snrcjt.cn

[Q43] 标量子查询
来源：http://eel.ydzc1.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dmx.snrcjt.cn

[Q44] IN 子查询
来源：http://phc.guowangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mzk.ppjwa.cn

[Q45] EXISTS 判断存在
来源：http://paf.nanxuanxn.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zob.pycfn.com

[Q46] NOT EXISTS 判断不存在
来源：http://mqc.jinqigufen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mtt.gzhubu.top

[Q47] 与平均值比较
来源：http://sgi.mhx1999.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ffw.9152youxi.cn

[Q48] CTE 公用表表达式
来源：http://fgf.chenjidiqi.icu

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://psm.mhx1999.top

SELECT * FROM t WHERE c > 5;
来源：http://xyf.zhongyouzk.top

[Q49] 更新单行
来源：http://ory.pengpengdd.cyou

UPDATE users SET status = 1 WHERE id = 10;
来源：http://okg.redwolf501.top

[Q50] 批量更新
来源：http://njx.xuanzx.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qiq.316326.xyz

[Q51] 用子查询更新
来源：http://gic.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://goi.redwolf501.top

[Q52] 删除指定行
来源：http://aic.zdqjudy.top

DELETE FROM users WHERE id = 10;
来源：http://aat.52xcode.cn

[Q53] 按条件删除
来源：http://npp.pycfn.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tij.vehdjk.com

[Q54] 清空表
来源：http://yel.gogol.net.cn

TRUNCATE TABLE logs;
来源：http://iwg.jyoumei.cn

[Q55] 排名（并列占位）
来源：http://khy.jinghuilouyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qik.wangdashe.top

[Q56] 密集排名（并列不占位）
来源：http://hoz.tanke756.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tkd.zhongyouzk.top

[Q57] 行号
来源：http://rqf.gzhubu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wro.ivvv.top

[Q58] 累计求和
来源：http://odd.shanyushiyangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tgj.ywan-chungtsiang.top

[Q59] 分组内累计
来源：http://rlm.cdnleiting.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lae.hcnkem.com

[Q60] 取上一行 / 下一行
来源：http://lce.c1oappe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ijo.zhongyouzk.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uhq.quarkkingdee.top

[Q61] 移动平均
来源：http://odq.ppjwa.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://djx.kuanghao11.cn

[Q62] 分组占比
来源：http://uox.gogol.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pkp.dianchejie.cn

[Q63] 开启事务
来源：http://hze.jqgfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://mzx.fanxiaobao.xyz

[Q64] 提交事务
来源：http://klf.jinghuilouyu.cn

COMMIT;
来源：http://vnl.xuetiantiany.cn

[Q65] 回滚事务
来源：http://lua.hesvh.cn

ROLLBACK;
来源：http://lva.kuanghao11.cn

[Q66] 行锁查询
来源：http://kkq.xinyue.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rtx.cashguo.top

[Q67] 设置隔离级别
来源：http://avz.0kj1m.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mpp.jinqigufen.top

[Q68] 保存点
来源：http://sfb.c1oappe.top

SAVEPOINT sp1;
来源：http://cbv.hysaishi.cn

ROLLBACK TO sp1;
来源：http://mno.zhengqikj.top

[Q69] 查看执行计划
来源：http://jwf.zycfv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bjw.ppjwa.cn

[Q70] 更新统计信息
来源：http://hze.ctjpmb.com

ANALYZE TABLE users;
来源：http://nhg.zhiwuduotai.top

[Q71] 查看建表语句
来源：http://fab.wangdashe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gcr.tanke756.top

[Q72] 查看索引
来源：http://jgn.zhongyouzk.top

SHOW INDEX FROM users;
来源：http://roe.fehbvm.com

[Q73] 查看表状态
来源：http://kti.quarkkingdee.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bki.jqgfzy.top

[Q74] 强制使用索引
来源：http://mfg.jianghu66.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rcf.yongpay.top

[Q75] 日期格式化
来源：http://odp.aizwys.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://iec.zhijiandao.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zku.jinghuilouyu.cn

[Q76] 按天统计
来源：http://qbp.daria6918.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://anh.jqgfzy.top

[Q77] 时间加减
来源：http://tzv.hnxiangtu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hws.zhixingplan.top

[Q78] 当前时间
来源：http://kbr.xuetiantiany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lnm.bjfxy.top

[Q79] 字符串拼接
来源：http://eas.zhixingplan.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yin.jinghuilouyu.cn

[Q80] 字符串截取
来源：http://zte.zhixingplan.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://syt.dashuyun.cn

[Q81] 字符串替换
来源：http://ivw.ywan-chungtsiang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vzc.zdbjq.cn

[Q82] 字符长度与字节长度
来源：http://vgy.yanxiufei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lsq.chenlongwang.top

[Q83] 大小写转换
来源：http://dqy.haohaochexian.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ugk.shuidangran.top

[Q84] 去除首尾空格
来源：http://wfu.ywan-chungtsiang.top

SELECT TRIM(name) FROM users;
来源：http://oqd.jinyuanbaomall.cn

[Q85] 数值取整
来源：http://zvs.vqdsnc.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dnc.chenzaomai.com

[Q86] 读取 JSON 字段
来源：http://fmg.yongpay.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wig.nanxinkj.top

[Q87] JSON 字段做条件
来源：http://xwu.hongshengwenyu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zee.epnwcf.com

[Q88] 行转列（条件聚合）
来源：http://rjb.jiagoushi.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kav.9152youxi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ips.chenlongwang.top

[Q89] 判断表是否存在
来源：http://tdw.tian-w.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://khn.nwbrower.top

[Q90] 生成序号列
来源：http://tlg.zhaomingkeji.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jwr.chenzaomai.com

================================================================================
来源：http://xun.cheryme.top

R. Bash 专题
来源：http://syn.chenzaomai.com

================================================================================
来源：http://yja.fanxiaobao.xyz

[R01] shebang 与严格模式
来源：http://ukb.zdqjudy.top

#!/usr/bin/env bash
来源：http://eoi.yangfankeji.com

set -euo pipefail
来源：http://zbs.pycfn.com

[R02] 变量赋值与使用
来源：http://tew.jqgufenzy.top

name="Tom"; echo "$name"
来源：http://shq.cheryme.top

[R03] 只读变量
来源：http://yfm.gogol.net.cn

readonly PI=3.14
来源：http://bgv.guannengcc.top

[R04] 位置参数
来源：http://vzf.birdmap.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wvs.svipenyu.cn

[R05] 参数默认值
来源：http://rae.yanxiufei.cn

name="${1:-default}"
来源：http://vof.wangshuangyany.cn

[R06] 判断命令是否存在
来源：http://vlf.cashguo.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fbv.yonumen.top

[R07] if 判断文件
来源：http://ehr.tianlin.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://veb.ivvv.top

[R08] 数值比较
来源：http://fmh.kuanghao11.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://csp.hysaishi.cn

[R09] 字符串比较
来源：http://uic.sweek.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://acs.yvedp.cn

[R10] 正则匹配
来源：http://qke.iojbl.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yow.fzhhl.top

[R11] case 多分支
来源：http://fcr.jinyuanbaomall.cn

case "$1" in
来源：http://epd.zhoulong.xyz

start) echo "启动" ;;
来源：http://wco.aibaodan.cn

stop)  echo "停止" ;;
来源：http://mxt.vqdsnc.cn

*)     echo "未知命令" ;;
来源：http://adh.sweek.top

esac
来源：http://jct.jianghu66.top

[R12] for 遍历文件
来源：http://fna.hnxiangtu.top

for f in *.txt; do echo "$f"; done
来源：http://pck.chenlongwang.top

[R13] for 计数循环
来源：http://dgx.andypj.xyz

for i in {1..10}; do echo "$i"; done
来源：http://amt.vqdsnc.cn

[R14] C 风格 for
来源：http://vye.fktsv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://asm.xinyue.icu

[R15] while 逐行读文件
来源：http://pel.gotoacloud.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gwi.nanxuanxn.top

[R16] until 等待条件
来源：http://hnd.yongpay.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wee.jyoumei.cn

[R17] 数组定义与取值
来源：http://ggv.svipenyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vjd.jianghu66.top

[R18] 遍历数组
来源：http://gbd.fanxiaobao.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://veh.ehwqpu.com

[R19] 数组长度
来源：http://cny.ybcxt.top

echo "${#arr[@]}"
来源：http://dfc.316326.xyz

[R20] 关联数组（字典）
来源：http://jgn.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qgm.hongshengwenyu.top

[R21] 字符串长度
来源：http://odx.yuxming.cn

echo "${#s}"
来源：http://xqq.yj20258.top

[R22] 截取子串
来源：http://mes.0kj1m.cn

echo "${s:0:5}"
来源：http://vnk.redwolf501.top

[R23] 字符串替换
来源：http://esq.aizwys.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kao.gaohongyu789.top

[R24] 大小写转换
来源：http://fws.yvedp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://umr.haohaochexian.top

[R25] 去后缀 / 去前缀
来源：http://lck.c1oappe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zcd.yueranfly.top

[R26] 命令替换
来源：http://xgc.bbcook.cn

now=$(date +%F); echo "$now"
来源：http://xkv.sxryk.cn

[R27] 算术展开
来源：http://mek.feifeiyinyue.top

echo $((1 + 2 * 3))
来源：http://oxo.epnwcf.com

[R28] 浮点运算
来源：http://mmq.jyoumei.cn

echo "scale=2; 10/3" | bc
来源：http://duf.vehdjk.com

[R29] 定义函数
来源：http://ayb.cdnleiting.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://evl.guowangkeji.top

[R30] 函数返回状态码
来源：http://amj.sufxvd.cn

f() { return 0; }; f || echo "失败了"
来源：http://wxi.zycfv.cn

[R31] 局部变量
来源：http://rec.cheryme.top

f() { local x=1; echo "$x"; }
来源：http://sao.nanxinkj.top

[R32] 参数个数校验
来源：http://cbc.nwbrower.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://goj.shanyushiyangkeji.top

[R33] 捕获错误并提示行号
来源：http://icv.xuanzx.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fbc.jiagoushi.top

[R34] 退出时清理
来源：http://ota.epnwcf.com

trap 'rm -f "$tmp"' EXIT
来源：http://lwp.nanxuanxn.top

[R35] 后台执行并等待
来源：http://svi.shangyingyoupin.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mct.quarkkingdee.top

[R36] 并发执行多个任务
来源：http://ibd.shanyushiyangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iyu.yanxiufei.cn

[R37] 把输出赋给变量
来源：http://rvz.andypj.xyz

files=$(ls -1)
来源：http://vtg.nanxuanxn.top

[R38] 管道串联
来源：http://cfo.dashuyun.cn

cat a.txt | grep -i error | wc -l
来源：http://kil.nwbrower.top

[R39] 重定向标准输出与错误
来源：http://jde.tarul.cn

cmd > out.log 2>&1
来源：http://kcf.iojbl.cn

[R40] 追加写日志
来源：http://tws.yuxming.cn

echo "log" >> out.log
来源：http://cdv.daria6918.cn

[R41] 丢弃输出
来源：http://xtw.nanxuanxn.top

cmd >/dev/null 2>&1
来源：http://pfs.zdqjudy.top

[R42] 输入重定向
来源：http://hri.ehwqpu.com

wc -l < a.txt
来源：http://kcj.wangdashe.top

[R43] 按名字查找文件
来源：http://uzg.zdqjudy.top

find . -name "*.log" -type f
来源：http://cse.havefunace.top

[R44] 按修改时间查找
来源：http://gft.316326.xyz

find . -mtime -7 -type f
来源：http://jcv.pycfn.com

[R45] 批量删除
来源：http://ltx.zhengqikj.top

find . -name "*.tmp" -delete
来源：http://ztp.hfpthk.cn

[R46] 递归替换文件内容
来源：http://prz.zhoulong.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hvq.ywan-chungtsiang.top

[R47] sed 单行替换
来源：http://iin.ppjwa.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hhz.pycfn.com

[R48] awk 取指定列
来源：http://ier.tianlin.xyz

awk '{print $1, $3}' a.txt
来源：http://tjc.tianlin.xyz

[R49] awk 带条件
来源：http://qat.andypj.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qpa.ppjwa.cn

[R50] awk 求和
来源：http://lxk.yj202588.top

awk '{s += $2} END {print s}' a.txt
来源：http://lkz.yueranfly.top

[R51] 排序去重取前几
来源：http://bcf.shuidangran.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cno.shzxlz.cn

[R52] 统计行数
来源：http://hmh.xziqi.cn

wc -l a.txt
来源：http://rgg.xylfe.cn

[R53] 查看文件头与实时尾
来源：http://vne.vqdsnc.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://biw.yuanzhike.top

[R54] 比较两个文件
来源：http://xee.ydjk.org.cn

diff a.txt b.txt
来源：http://dmj.fanxiaobao.xyz

[R55] 压缩与解压
来源：http://nzi.andypj.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ayn.xuetiantiany.cn

[R56] 远程拷贝
来源：http://cpz.zhijiandao.cn

scp file user@host:/path/
来源：http://rla.sufxvd.cn

[R57] 远程执行命令
来源：http://dgy.tanke756.top

ssh user@host 'uptime'
来源：http://sda.vehdjk.com

[R58] 下载文件
来源：http://gae.mhx1999.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mbl.ivvv.top

[R59] 发 POST JSON
来源：http://fnc.tianlin.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bfw.guannengcc.top

[R60] 只看 HTTP 状态码
来源：http://dco.svipenyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iaz.jinyuanbaomall.cn

[R61] 磁盘占用
来源：http://pna.fehbvm.com

df -h;  du -sh *
来源：http://mkg.ywan-chungtsiang.top

[R62] 找最占空间的文件
来源：http://dwt.tarul.cn

du -ah . | sort -rh | head -10
来源：http://nwp.gzhubu.top

[R63] 内存与进程
来源：http://hgl.hnxiangtu.top

free -h;  ps aux | grep nginx
来源：http://gcp.shuidangran.top

[R64] 结束进程
来源：http://evo.ehwqpu.com

kill -9 $(pgrep -f app.py)
来源：http://jzk.hammf.cn

[R65] 查看端口占用
来源：http://daq.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ozz.cdnleiting.top

[R66] 定时任务
来源：http://tdv.gzhubu.top

crontab -e;  crontab -l
来源：http://wsf.pengpengdd.cyou

[R67] 生成随机十六进制串
来源：http://ghw.meibo888.top

openssl rand -hex 16
来源：http://xyd.redwolf501.top

[R68] 计算文件校验值
来源：http://ogk.kuanghao11.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yah.hammf.cn

[R69] 生成随机密码
来源：http://hjh.zdbjq.cn

head -c 16 /dev/urandom | base64
来源：http://htr.ctjpmb.com

[R70] 时间戳与互转
来源：http://xrr.yj202588.top

date +%s;  date -d @1700000000
来源：http://phe.guannengcc.top

[R71] 日期格式化
来源：http://rwu.316326.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://kzp.nanxuanxn.top

[R72] 等待端口就绪
来源：http://hao.svipenyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qvf.jinqigfzy.top

[R73] 分割大日志
来源：http://jnv.chenjidiqi.icu

split -l 1000 big.log part_
来源：http://lfq.yongpay.top

[R74] 批量重命名
来源：http://kfx.zhaomingkeji.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://isr.yuxming.cn

[R75] 导出环境变量
来源：http://fpg.bjfxy.top

export PATH="$HOME/bin:$PATH"
来源：http://ddl.zhengqikj.top

[R76] 使用临时文件
来源：http://vuh.gzhubu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xuc.fzhhl.top

[R77] 读取用户输入
来源：http://guu.sweek.top

read -rp "请输入: " ans
来源：http://ass.gaohongyu789.top

[R78] 交互式菜单
来源：http://bae.meibo888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ruw.cucudq.cn

[R79] 解析命令行选项
来源：http://gxh.ivvv.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vbj.sweek.top

[R80] 查看脚本执行耗时
来源：http://avo.uphjek.com

time ./run.sh
来源：http://taq.sweek.top

================================================================================
来源：http://tzh.hnxiangtu.top

S. C / C++ 专题
来源：http://qhl.ywan-chungtsiang.top

================================================================================
来源：http://jxh.bbcook.cn

[S01] C：Hello World
来源：http://kwg.316326.xyz

#include <stdio.h>
来源：http://aij.yj20258888.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nzy.yuanzhike.top

[S02] C：变量与格式化输出
来源：http://cju.tarul.cn

int a = 10; printf("%d\n", a);
来源：http://rgp.zhongyouzk.top

[S03] C：读入整数
来源：http://glv.jinghuilouyu.cn

int x; scanf("%d", &x);
来源：http://gus.smart0.xyz

[S04] C：字符串复制
来源：http://oyi.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://dvl.cucudq.cn

[S05] C：字符串长度
来源：http://bbv.vehdjk.com

strlen(s)
来源：http://zss.hongshengwenyu.top

[S06] C：字符串比较
来源：http://dax.hongshengwenyu.top

strcmp(a, b) == 0
来源：http://bho.gotoacloud.top

[S07] C：数组遍历求和
来源：http://dvk.hcnkem.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bqw.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://jwh.nanxuanxn.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oyw.vehdjk.com

[S09] C：结构体定义与初始化
来源：http://gxv.fanxiaobao.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mjk.cucudq.cn

[S10] C：指针与解引用
来源：http://und.jinghuilouyu.cn

int *p = &a;  *p = 5;
来源：http://fvo.yongpay.top

[S11] C：逐行读文件
来源：http://qwt.zhixingplan.top


<!-- 参考信息 -->