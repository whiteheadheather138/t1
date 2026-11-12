代发 wailian999

[Q44] IN 子查询
来源：http://fdb.ctjpmb.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ahs.chenjidiqi.icu

[Q45] EXISTS 判断存在
来源：http://mlg.yj20258888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://arh.hnqzz.top

[Q46] NOT EXISTS 判断不存在
来源：http://erc.shzxlz.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uoa.fktsv.cn

[Q47] 与平均值比较
来源：http://cqq.yvedp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://omx.zdbjq.cn

[Q48] CTE 公用表表达式
来源：http://kpm.daria6918.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pjs.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://dnn.xuetiantiany.cn

[Q49] 更新单行
来源：http://ufn.c1oappe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uhk.hammf.cn

[Q50] 批量更新
来源：http://kma.fanxiaobao.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sta.yuxming.cn

[Q51] 用子查询更新
来源：http://sct.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://icg.hywenlv.cn

[Q52] 删除指定行
来源：http://jrq.yongpay.top

DELETE FROM users WHERE id = 10;
来源：http://ccf.jyoumei.cn

[Q53] 按条件删除
来源：http://fyh.yuanzhike.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vsu.smart0.xyz

[Q54] 清空表
来源：http://asj.quarkkingdee.top

TRUNCATE TABLE logs;
来源：http://gof.tianlin.xyz

[Q55] 排名（并列占位）
来源：http://cqx.tianlin.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://swp.yj20258888.top

[Q56] 密集排名（并列不占位）
来源：http://huw.aizwys.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://agp.redwolf501.top

[Q57] 行号
来源：http://mfy.chenlongwang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://igr.zhiwuduotai.top

[Q58] 累计求和
来源：http://lba.feifeiyinyue.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tpx.fengsongda.top

[Q59] 分组内累计
来源：http://xqo.aibaodan.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kkc.hnxiangtu.top

[Q60] 取上一行 / 下一行
来源：http://qig.shzxlz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rmh.nwbrower.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vad.hfpthk.cn

[Q61] 移动平均
来源：http://egc.kuanghao11.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ewq.yueranfly.top

[Q62] 分组占比
来源：http://ojh.andypj.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sfq.sysykeji.top

[Q63] 开启事务
来源：http://rrp.shzxlz.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://btz.jiagoushi.top

[Q64] 提交事务
来源：http://obv.feifeiyinyue.top

COMMIT;
来源：http://dmf.jiagoushi.top

[Q65] 回滚事务
来源：http://rto.jinyuanbaomall.cn

ROLLBACK;
来源：http://eph.yj20258.top

[Q66] 行锁查询
来源：http://rpd.yongpay.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qez.9152youxi.cn

[Q67] 设置隔离级别
来源：http://xnt.ppjwa.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lnd.tanke756.top

[Q68] 保存点
来源：http://ons.zdbjq.cn

SAVEPOINT sp1;
来源：http://ztx.ctjpmb.com

ROLLBACK TO sp1;
来源：http://scx.shanyushiyangkeji.top

[Q69] 查看执行计划
来源：http://ilq.xuetiantiany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nwi.iojbl.cn

[Q70] 更新统计信息
来源：http://lhr.fanxiaobao.xyz

ANALYZE TABLE users;
来源：http://irf.sufxvd.cn

[Q71] 查看建表语句
来源：http://bfl.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xnz.ywan-chungtsiang.top

[Q72] 查看索引
来源：http://xyr.ybcxt.top

SHOW INDEX FROM users;
来源：http://ezv.ehwqpu.com

[Q73] 查看表状态
来源：http://tmu.quarkkingdee.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ous.bjfxy.top

[Q74] 强制使用索引
来源：http://kaf.shanyushiyangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ezf.guannengcc.top

[Q75] 日期格式化
来源：http://ojy.tanke756.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hee.pengpengdd.cyou

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nqa.zdqjudy.top

[Q76] 按天统计
来源：http://rqh.0kj1m.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://geo.0kj1m.cn

[Q77] 时间加减
来源：http://kho.jinyuanbaomall.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fft.mhx1999.top

[Q78] 当前时间
来源：http://jwq.yanxiufei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rqm.zycfv.cn

[Q79] 字符串拼接
来源：http://rmp.jqgufenzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://osu.hongshengwenyu.top

[Q80] 字符串截取
来源：http://zhf.zhixingplan.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://waw.havefunace.top

[Q81] 字符串替换
来源：http://gpb.sysykeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jsk.zhaomingkeji.xyz

[Q82] 字符长度与字节长度
来源：http://zfk.shanyushiyangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ocu.uphjek.com

[Q83] 大小写转换
来源：http://lzk.fzhhl.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fqk.52xcode.cn

[Q84] 去除首尾空格
来源：http://sfg.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://uet.yongpay.top

[Q85] 数值取整
来源：http://mng.zhixingplan.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vxz.guowangkeji.top

[Q86] 读取 JSON 字段
来源：http://jqj.ehwqpu.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jqo.shanyushiyangtech.top

[Q87] JSON 字段做条件
来源：http://mxo.c1oappe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zew.zycfv.cn

[Q88] 行转列（条件聚合）
来源：http://fnz.meibo888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://peo.dianchejie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ymq.fanxiaobao.xyz

[Q89] 判断表是否存在
来源：http://dey.pycfn.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://akt.cashguo.top

[Q90] 生成序号列
来源：http://vup.vehdjk.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pih.316326.xyz

================================================================================
来源：http://nse.xuanzx.com

R. Bash 专题
来源：http://lww.hongshengwenyu.top

================================================================================
来源：http://str.tian-w.cn

[R01] shebang 与严格模式
来源：http://qen.chenjidiqi.icu

#!/usr/bin/env bash
来源：http://ogp.hesvh.cn

set -euo pipefail
来源：http://zsz.bjfxy.top

[R02] 变量赋值与使用
来源：http://jaj.gogol.net.cn

name="Tom"; echo "$name"
来源：http://lmg.hammf.cn

[R03] 只读变量
来源：http://div.jiagoushi.top

readonly PI=3.14
来源：http://lux.fktsv.cn

[R04] 位置参数
来源：http://bha.gzhubu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uvt.yueranfly.top

[R05] 参数默认值
来源：http://nbc.andypj.xyz

name="${1:-default}"
来源：http://bvy.yuanzhike.top

[R06] 判断命令是否存在
来源：http://sjs.zhoulong.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://twm.dashuyun.cn

[R07] if 判断文件
来源：http://faj.jinqigufen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xat.ybcxt.top

[R08] 数值比较
来源：http://jna.xinyue.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://ffi.cheryme.top

[R09] 字符串比较
来源：http://nah.yonumen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hyt.zdqjudy.top

[R10] 正则匹配
来源：http://gox.c1oappe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bse.quarkkingdee.top

[R11] case 多分支
来源：http://ggq.yvedp.cn

case "$1" in
来源：http://aga.yj20258888.top

start) echo "启动" ;;
来源：http://wrs.shangyingyoupin.top

stop)  echo "停止" ;;
来源：http://lmk.zdqjudy.top

*)     echo "未知命令" ;;
来源：http://ckb.meibo888.top

esac
来源：http://dmx.quarkkingdee.top

[R12] for 遍历文件
来源：http://oog.fanxiaobao.xyz

for f in *.txt; do echo "$f"; done
来源：http://mqk.chenlongwang.top

[R13] for 计数循环
来源：http://ppr.cheryme.top

for i in {1..10}; do echo "$i"; done
来源：http://ave.mhx1999.top

[R14] C 风格 for
来源：http://xzk.nwbrower.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yiw.ydzc1.top

[R15] while 逐行读文件
来源：http://lkn.redwolf501.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://afb.fengsongda.top

[R16] until 等待条件
来源：http://rof.yj20258888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hsz.yj202588.top

[R17] 数组定义与取值
来源：http://ynv.vehdjk.com

arr=(a b c); echo "${arr[0]}"
来源：http://cfl.zycfv.cn

[R18] 遍历数组
来源：http://ljz.chenzaomai.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lyg.cdnleiting.top

[R19] 数组长度
来源：http://bce.0kj1m.cn

echo "${#arr[@]}"
来源：http://wyn.yangfankeji.com

[R20] 关联数组（字典）
来源：http://pfd.iojbl.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jez.fanxiaobao.xyz

[R21] 字符串长度
来源：http://ogt.cheryme.top

echo "${#s}"
来源：http://jyl.52xcode.cn

[R22] 截取子串
来源：http://fbr.andypj.xyz

echo "${s:0:5}"
来源：http://qgr.yuanzhike.top

[R23] 字符串替换
来源：http://gfn.jqgfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nhb.hfpthk.cn

[R24] 大小写转换
来源：http://cxa.vehdjk.com

echo "${s^^}"; echo "${s,,}"
来源：http://tak.nanxuanxn.top

[R25] 去后缀 / 去前缀
来源：http://sym.jlsjyb.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bxe.xylfe.cn

[R26] 命令替换
来源：http://xqo.xuanzx.com

now=$(date +%F); echo "$now"
来源：http://oah.havefunace.top

[R27] 算术展开
来源：http://bwc.xuetiantiany.cn

echo $((1 + 2 * 3))
来源：http://ciz.uphjek.com

[R28] 浮点运算
来源：http://qci.jqgfzy.top

echo "scale=2; 10/3" | bc
来源：http://kmy.shangyingyoupin.top

[R29] 定义函数
来源：http://rqm.yongpay.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tmv.chenzaomai.com

[R30] 函数返回状态码
来源：http://yoh.kuanghao11.cn

f() { return 0; }; f || echo "失败了"
来源：http://clh.nanxinkj.top

[R31] 局部变量
来源：http://ucs.zdqjudy.top

f() { local x=1; echo "$x"; }
来源：http://svz.zdbjq.cn

[R32] 参数个数校验
来源：http://eju.pycfn.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kim.gotoacloud.top

[R33] 捕获错误并提示行号
来源：http://ccy.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dzu.shzxlz.cn

[R34] 退出时清理
来源：http://myb.fengsongda.top

trap 'rm -f "$tmp"' EXIT
来源：http://oxt.xziqi.cn

[R35] 后台执行并等待
来源：http://oqq.hcnkem.com

sleep 5 & pid=$!; wait "$pid"
来源：http://ity.zhijiandao.cn

[R36] 并发执行多个任务
来源：http://kov.cashguo.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yfy.jqgfzy.top

[R37] 把输出赋给变量
来源：http://wrt.uphjek.com

files=$(ls -1)
来源：http://fup.ivvv.top

[R38] 管道串联
来源：http://llo.hongshengwenyu.top

cat a.txt | grep -i error | wc -l
来源：http://xsk.yfazqb.com

[R39] 重定向标准输出与错误
来源：http://boj.feifeiyinyue.top

cmd > out.log 2>&1
来源：http://zrq.gotoacloud.top

[R40] 追加写日志
来源：http://qew.fktsv.cn

echo "log" >> out.log
来源：http://quu.quarkkingdee.top

[R41] 丢弃输出
来源：http://auf.cashguo.top

cmd >/dev/null 2>&1
来源：http://bks.xylfe.cn

[R42] 输入重定向
来源：http://irv.52xcode.cn

wc -l < a.txt
来源：http://sgw.zhiwuduotai.top

[R43] 按名字查找文件
来源：http://jlb.fzhhl.top

find . -name "*.log" -type f
来源：http://gek.ybcxt.top

[R44] 按修改时间查找
来源：http://wek.tanke756.top

find . -mtime -7 -type f
来源：http://rmr.hongshengwenyu.top

[R45] 批量删除
来源：http://ixr.hywenlv.cn

find . -name "*.tmp" -delete
来源：http://bsx.svipenyu.cn

[R46] 递归替换文件内容
来源：http://lcz.zhaomingkeji.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eqw.aizwys.cn

[R47] sed 单行替换
来源：http://gtz.0kj1m.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bhd.pengpengdd.cyou

[R48] awk 取指定列
来源：http://uqz.zhiwuduotai.top

awk '{print $1, $3}' a.txt
来源：http://vly.yongpay.top

[R49] awk 带条件
来源：http://ocx.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qnq.guowangkeji.top

[R50] awk 求和
来源：http://tzh.shanyushiyangtech.top

awk '{s += $2} END {print s}' a.txt
来源：http://cms.jiagoushi.top

[R51] 排序去重取前几
来源：http://fkx.ydjk.org.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vpx.fengsongda.top

[R52] 统计行数
来源：http://wlr.redwolf501.top

wc -l a.txt
来源：http://tnb.yongpay.top

[R53] 查看文件头与实时尾
来源：http://iag.nanxuanxn.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rxh.haohaochexian.top

[R54] 比较两个文件
来源：http://zdi.ybcxt.top

diff a.txt b.txt
来源：http://dru.hongshengwenyu.top

[R55] 压缩与解压
来源：http://gfb.fanxiaobao.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://klm.0kj1m.cn

[R56] 远程拷贝
来源：http://fdp.haohaochexian.top

scp file user@host:/path/
来源：http://jor.snrcjt.cn

[R57] 远程执行命令
来源：http://bvz.tanke756.top

ssh user@host 'uptime'
来源：http://yqn.cashguo.top

[R58] 下载文件
来源：http://grh.ehwqpu.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sai.jianghu66.top

[R59] 发 POST JSON
来源：http://dwh.wangshuangyany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tor.birdmap.top

[R60] 只看 HTTP 状态码
来源：http://evz.aizwys.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wth.jlsjyb.cn

[R61] 磁盘占用
来源：http://lds.jlsjyb.cn

df -h;  du -sh *
来源：http://pgs.iojbl.cn

[R62] 找最占空间的文件
来源：http://lkz.cashguo.top

du -ah . | sort -rh | head -10
来源：http://iss.hnxiangtu.top

[R63] 内存与进程
来源：http://esh.shuidangran.top

free -h;  ps aux | grep nginx
来源：http://axz.xinyue.icu

[R64] 结束进程
来源：http://exr.meibo888.top

kill -9 $(pgrep -f app.py)
来源：http://zof.smart0.xyz

[R65] 查看端口占用
来源：http://amr.yj20258.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vtk.smart0.xyz

[R66] 定时任务
来源：http://muf.aibaodan.cn

crontab -e;  crontab -l
来源：http://adk.hongshengwenyu.top

[R67] 生成随机十六进制串
来源：http://ixj.hywenlv.cn

openssl rand -hex 16
来源：http://qxw.zhaomingkeji.xyz

[R68] 计算文件校验值
来源：http://umj.ybcxt.top

sha256sum a.txt;  md5sum a.txt
来源：http://odk.zhijiandao.cn

[R69] 生成随机密码
来源：http://llg.nanxinkj.top

head -c 16 /dev/urandom | base64
来源：http://jim.feifeiyinyue.top

[R70] 时间戳与互转
来源：http://wle.yvedp.cn

date +%s;  date -d @1700000000
来源：http://vgb.jianghu66.top

[R71] 日期格式化
来源：http://gmk.fengsongda.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qje.sysykeji.top

[R72] 等待端口就绪
来源：http://bay.svipenyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://unj.haohaochexian.top

[R73] 分割大日志
来源：http://dfb.ppjwa.cn

split -l 1000 big.log part_
来源：http://rpy.fanxiaobao.xyz

[R74] 批量重命名
来源：http://hao.zhongyouzk.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qli.zdbjq.cn

[R75] 导出环境变量
来源：http://aiu.yj20258.top

export PATH="$HOME/bin:$PATH"
来源：http://ipx.gogol.net.cn

[R76] 使用临时文件
来源：http://kiz.zhongyouzk.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oqz.dianchejie.cn

[R77] 读取用户输入
来源：http://paq.quarkkingdee.top

read -rp "请输入: " ans
来源：http://mof.sxryk.cn

[R78] 交互式菜单
来源：http://vsl.gzhubu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ivk.zhoulong.xyz

[R79] 解析命令行选项
来源：http://jwt.andypj.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hhq.gogol.net.cn

[R80] 查看脚本执行耗时
来源：http://vfq.nanxuanxn.top

time ./run.sh
来源：http://tzl.jinqigufen.top

================================================================================
来源：http://zol.0kj1m.cn

S. C / C++ 专题
来源：http://iqh.xziqi.cn

================================================================================
来源：http://kfu.yj20258.top

[S01] C：Hello World
来源：http://kba.xuanzx.com

#include <stdio.h>
来源：http://ejb.shuidangran.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://tnc.havefunace.top

[S02] C：变量与格式化输出
来源：http://ehl.gzhubu.top

int a = 10; printf("%d\n", a);
来源：http://ncf.pycfn.com

[S03] C：读入整数
来源：http://gbi.jqgufenzy.top

int x; scanf("%d", &x);
来源：http://tki.xuanzx.com

[S04] C：字符串复制
来源：http://tls.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://hro.hysaishi.cn

[S05] C：字符串长度
来源：http://pzb.xziqi.cn

strlen(s)
来源：http://nlm.jlsjyb.cn

[S06] C：字符串比较
来源：http://pbq.shuidangran.top

strcmp(a, b) == 0
来源：http://uuo.redwolf501.top

[S07] C：数组遍历求和
来源：http://oiy.quarkkingdee.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://diy.jqgufenzy.top

[S08] C：动态内存分配与释放
来源：http://mta.shzxlz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bzc.fehbvm.com

[S09] C：结构体定义与初始化
来源：http://ftg.xziqi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ilh.c1oappe.top

[S10] C：指针与解引用
来源：http://sso.zhaomingkeji.xyz

int *p = &a;  *p = 5;
来源：http://dwn.vehdjk.com

[S11] C：逐行读文件
来源：http://imc.sjlbkw.cn

FILE *f = fopen("a.txt", "r");
来源：http://fmu.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rmj.hfpthk.cn

fclose(f);
来源：http://vrb.vehdjk.com

[S12] C：写文件
来源：http://bef.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://elx.c1oappe.top

[S13] C：宏定义
来源：http://dgl.gotoacloud.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qng.zhoulong.xyz

[S14] C：枚举
来源：http://zml.nanxuanxn.top


<!-- 参考信息 -->