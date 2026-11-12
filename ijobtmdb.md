代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://cue.bjfxy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dob.ivvv.top

[Q47] 与平均值比较
来源：http://yya.yongpay.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lmb.mhx1999.top

[Q48] CTE 公用表表达式
来源：http://wpq.pycfn.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jyc.zycfv.cn

SELECT * FROM t WHERE c > 5;
来源：http://mwl.fktsv.cn

[Q49] 更新单行
来源：http://zdf.yanxiufei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qum.yanxiufei.cn

[Q50] 批量更新
来源：http://goj.andypj.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rdi.jinyuanbaomall.cn

[Q51] 用子查询更新
来源：http://def.chenzaomai.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lbn.yj202588.top

[Q52] 删除指定行
来源：http://iyn.zycfv.cn

DELETE FROM users WHERE id = 10;
来源：http://xlj.jqgufenzy.top

[Q53] 按条件删除
来源：http://opp.gotoacloud.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sjp.pycfn.com

[Q54] 清空表
来源：http://hio.jianghu66.top

TRUNCATE TABLE logs;
来源：http://wyn.ehwqpu.com

[Q55] 排名（并列占位）
来源：http://hiu.zhoulong.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xgn.yfazqb.com

[Q56] 密集排名（并列不占位）
来源：http://zyj.sjlbkw.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tyz.fengsongda.top

[Q57] 行号
来源：http://ayu.9152youxi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mmu.fehbvm.com

[Q58] 累计求和
来源：http://lat.feifeiyinyue.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://phc.birdmap.top

[Q59] 分组内累计
来源：http://lmx.hysaishi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mxe.daria6918.cn

[Q60] 取上一行 / 下一行
来源：http://oih.jinghuilouyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ifn.hnqzz.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qeh.xylfe.cn

[Q61] 移动平均
来源：http://rii.hywenlv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://awy.xuanzx.com

[Q62] 分组占比
来源：http://kdb.ctjpmb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://apc.svipenyu.cn

[Q63] 开启事务
来源：http://khq.fzhhl.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tdw.ivvv.top

[Q64] 提交事务
来源：http://vwj.dashuyun.cn

COMMIT;
来源：http://zgs.snrcjt.cn

[Q65] 回滚事务
来源：http://fgt.c1oappe.top

ROLLBACK;
来源：http://bhx.gaohongyu789.top

[Q66] 行锁查询
来源：http://rgf.hesvh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://koq.jqgfzy.top

[Q67] 设置隔离级别
来源：http://kic.jqgufenzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lke.yonumen.top

[Q68] 保存点
来源：http://eay.jlsjyb.cn

SAVEPOINT sp1;
来源：http://bsv.zhiwuduotai.top

ROLLBACK TO sp1;
来源：http://qmi.tianlin.xyz

[Q69] 查看执行计划
来源：http://jmi.fktsv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sch.zhiwuduotai.top

[Q70] 更新统计信息
来源：http://zeq.pengpengdd.cyou

ANALYZE TABLE users;
来源：http://ovg.tarul.cn

[Q71] 查看建表语句
来源：http://emr.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kum.fzhhl.top

[Q72] 查看索引
来源：http://dny.zycfv.cn

SHOW INDEX FROM users;
来源：http://lco.ppjwa.cn

[Q73] 查看表状态
来源：http://dvo.jyoumei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ruv.yj202588.top

[Q74] 强制使用索引
来源：http://neg.xuetiantiany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yzr.zdqjudy.top

[Q75] 日期格式化
来源：http://vcm.sweek.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://oqm.tianlin.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nzy.yvedp.cn

[Q76] 按天统计
来源：http://lkq.sweek.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pvs.tianlin.xyz

[Q77] 时间加减
来源：http://bqd.aibaodan.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xhk.andypj.xyz

[Q78] 当前时间
来源：http://pwh.0kj1m.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://whw.tarul.cn

[Q79] 字符串拼接
来源：http://czf.uphjek.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qqv.pengpengdd.cyou

[Q80] 字符串截取
来源：http://tdc.fengsongda.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://izw.dianchejie.cn

[Q81] 字符串替换
来源：http://cwf.jianghu66.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jpt.hysaishi.cn

[Q82] 字符长度与字节长度
来源：http://kjp.ppjwa.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://szk.ydjk.org.cn

[Q83] 大小写转换
来源：http://xjc.vqdsnc.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://spf.zdqjudy.top

[Q84] 去除首尾空格
来源：http://evz.tarul.cn

SELECT TRIM(name) FROM users;
来源：http://bjt.jinghuilouyu.cn

[Q85] 数值取整
来源：http://gvs.hywenlv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tgn.tanke756.top

[Q86] 读取 JSON 字段
来源：http://snh.yvedp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zbr.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://spe.vqdsnc.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://weq.nanxinkj.top

[Q88] 行转列（条件聚合）
来源：http://bst.gotoacloud.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qfd.xuetiantiany.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ltf.uphjek.com

[Q89] 判断表是否存在
来源：http://kvi.ywan-chungtsiang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tjt.fktsv.cn

[Q90] 生成序号列
来源：http://cid.chenjidiqi.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://avv.xylfe.cn

================================================================================
来源：http://dtr.jyoumei.cn

R. Bash 专题
来源：http://cph.zhijiandao.cn

================================================================================
来源：http://sbj.hcnkem.com

[R01] shebang 与严格模式
来源：http://gag.kuanghao11.cn

#!/usr/bin/env bash
来源：http://toe.hcnkem.com

set -euo pipefail
来源：http://emf.yj202588.top

[R02] 变量赋值与使用
来源：http://hck.epnwcf.com

name="Tom"; echo "$name"
来源：http://sks.zhoulong.xyz

[R03] 只读变量
来源：http://sir.redwolf501.top

readonly PI=3.14
来源：http://oye.yj202588.top

[R04] 位置参数
来源：http://aef.guannengcc.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qtc.shzxlz.cn

[R05] 参数默认值
来源：http://xqx.yueranfly.top

name="${1:-default}"
来源：http://hig.ybcxt.top

[R06] 判断命令是否存在
来源：http://ull.redwolf501.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gts.guannengcc.top

[R07] if 判断文件
来源：http://jux.ehwqpu.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://euy.fanxiaobao.xyz

[R08] 数值比较
来源：http://gat.pengpengdd.cyou

if (( a > b )); then echo "a 更大"; fi
来源：http://tdm.tarul.cn

[R09] 字符串比较
来源：http://huh.daxiang520.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uvs.zhixingplan.top

[R10] 正则匹配
来源：http://dfz.cashguo.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jfy.sufxvd.cn

[R11] case 多分支
来源：http://gla.uphjek.com

case "$1" in
来源：http://kat.andypj.xyz

start) echo "启动" ;;
来源：http://yew.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://nbd.jinqigfzy.top

*)     echo "未知命令" ;;
来源：http://rwv.zdqjudy.top

esac
来源：http://ptw.epnwcf.com

[R12] for 遍历文件
来源：http://qrq.fktsv.cn

for f in *.txt; do echo "$f"; done
来源：http://ogb.sxryk.cn

[R13] for 计数循环
来源：http://dlo.jqgufenzy.top

for i in {1..10}; do echo "$i"; done
来源：http://vwn.daxiang520.top

[R14] C 风格 for
来源：http://qoe.jyoumei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qjb.sjlbkw.cn

[R15] while 逐行读文件
来源：http://rcv.zhoulong.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tye.jqgufenzy.top

[R16] until 等待条件
来源：http://grp.xinyue.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qch.jinyuanbaomall.cn

[R17] 数组定义与取值
来源：http://pbl.hywenlv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://byw.tianlin.xyz

[R18] 遍历数组
来源：http://lfm.feifeiyinyue.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yny.yuanzhike.top

[R19] 数组长度
来源：http://aja.zhiwuduotai.top

echo "${#arr[@]}"
来源：http://smz.tanke756.top

[R20] 关联数组（字典）
来源：http://jcm.tanke756.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bov.vehdjk.com

[R21] 字符串长度
来源：http://hvu.jlsjyb.cn

echo "${#s}"
来源：http://zil.tianlin.xyz

[R22] 截取子串
来源：http://uti.hammf.cn

echo "${s:0:5}"
来源：http://hqb.fzhhl.top

[R23] 字符串替换
来源：http://bwd.aizwys.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tkg.xylfe.cn

[R24] 大小写转换
来源：http://gag.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://tcj.uphjek.com

[R25] 去后缀 / 去前缀
来源：http://ngn.zhaomingkeji.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://vns.dianchejie.cn

[R26] 命令替换
来源：http://cub.ywan-chungtsiang.top

now=$(date +%F); echo "$now"
来源：http://map.hnqzz.top

[R27] 算术展开
来源：http://nnf.mhx1999.top

echo $((1 + 2 * 3))
来源：http://inx.316326.xyz

[R28] 浮点运算
来源：http://ylq.svipenyu.cn

echo "scale=2; 10/3" | bc
来源：http://gif.zhijiandao.cn

[R29] 定义函数
来源：http://slj.yj20258.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zuv.mhx1999.top

[R30] 函数返回状态码
来源：http://pgq.yj20258.top

f() { return 0; }; f || echo "失败了"
来源：http://che.fengsongda.top

[R31] 局部变量
来源：http://apf.pengpengdd.cyou

f() { local x=1; echo "$x"; }
来源：http://nso.chenlongwang.top

[R32] 参数个数校验
来源：http://cdr.fehbvm.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bvj.haohaochexian.top

[R33] 捕获错误并提示行号
来源：http://xzl.wangshuangyany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uch.hongshengwenyu.top

[R34] 退出时清理
来源：http://egm.ywan-chungtsiang.top

trap 'rm -f "$tmp"' EXIT
来源：http://its.daria6918.cn

[R35] 后台执行并等待
来源：http://sic.vehdjk.com

sleep 5 & pid=$!; wait "$pid"
来源：http://aii.jlsjyb.cn

[R36] 并发执行多个任务
来源：http://cfr.zhengqikj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xif.wangdashe.top

[R37] 把输出赋给变量
来源：http://ujs.bjfxy.top

files=$(ls -1)
来源：http://rmw.jinghuilouyu.cn

[R38] 管道串联
来源：http://iej.tianlin.xyz

cat a.txt | grep -i error | wc -l
来源：http://hcs.xingfuxueyuan.xyz

[R39] 重定向标准输出与错误
来源：http://jhh.guannengcc.top

cmd > out.log 2>&1
来源：http://hap.cucudq.cn

[R40] 追加写日志
来源：http://zvi.haohaochexian.top

echo "log" >> out.log
来源：http://xso.cashguo.top

[R41] 丢弃输出
来源：http://tlh.wangshuangyany.cn

cmd >/dev/null 2>&1
来源：http://inh.jqgfzy.top

[R42] 输入重定向
来源：http://vlk.fanxiaobao.xyz

wc -l < a.txt
来源：http://yit.nwbrower.top

[R43] 按名字查找文件
来源：http://bqe.xuetiantiany.cn

find . -name "*.log" -type f
来源：http://hkn.jqgfzy.top

[R44] 按修改时间查找
来源：http://ytb.cqqwz.cn

find . -mtime -7 -type f
来源：http://hzs.nanxinkj.top

[R45] 批量删除
来源：http://zis.jiagoushi.top

find . -name "*.tmp" -delete
来源：http://fmk.svipenyu.cn

[R46] 递归替换文件内容
来源：http://yfz.mhx1999.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://svy.fktsv.cn

[R47] sed 单行替换
来源：http://wez.shanyushiyangtech.top

sed -i 's/foo/bar/g' a.txt
来源：http://kap.sjlbkw.cn

[R48] awk 取指定列
来源：http://upg.daxiang520.top

awk '{print $1, $3}' a.txt
来源：http://uxz.tanke756.top

[R49] awk 带条件
来源：http://hto.ppjwa.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://boc.fanxiaobao.xyz

[R50] awk 求和
来源：http://jse.andypj.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://geo.yj20258888.top

[R51] 排序去重取前几
来源：http://wbo.tarul.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fqr.pengpengdd.cyou

[R52] 统计行数
来源：http://tbj.jinqigfzy.top

wc -l a.txt
来源：http://ptk.hesvh.cn

[R53] 查看文件头与实时尾
来源：http://hfh.zycfv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kra.yongpay.top

[R54] 比较两个文件
来源：http://pnz.meibo888.top

diff a.txt b.txt
来源：http://gir.vehdjk.com

[R55] 压缩与解压
来源：http://pqc.fzhhl.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://brs.mhx1999.top

[R56] 远程拷贝
来源：http://irj.dashuyun.cn

scp file user@host:/path/
来源：http://efk.c1oappe.top

[R57] 远程执行命令
来源：http://hry.jyoumei.cn

ssh user@host 'uptime'
来源：http://qli.ehwqpu.com

[R58] 下载文件
来源：http://odu.yvedp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wmc.daxiang520.top

[R59] 发 POST JSON
来源：http://aar.zhoulong.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dsc.birdmap.top

[R60] 只看 HTTP 状态码
来源：http://zyt.hcnkem.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://awp.sysykeji.top

[R61] 磁盘占用
来源：http://feq.yanxiufei.cn

df -h;  du -sh *
来源：http://rbh.jinghuilouyu.cn

[R62] 找最占空间的文件
来源：http://amt.316326.xyz

du -ah . | sort -rh | head -10
来源：http://edt.shanyushiyangtech.top

[R63] 内存与进程
来源：http://piq.fanxiaobao.xyz

free -h;  ps aux | grep nginx
来源：http://aoe.cdnleiting.top

[R64] 结束进程
来源：http://hls.tian-w.cn

kill -9 $(pgrep -f app.py)
来源：http://eqq.fengsongda.top

[R65] 查看端口占用
来源：http://fsz.ivvv.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jux.nanxuanxn.top

[R66] 定时任务
来源：http://ecy.xylfe.cn

crontab -e;  crontab -l
来源：http://mnu.shanyushiyangkeji.top

[R67] 生成随机十六进制串
来源：http://ael.havefunace.top

openssl rand -hex 16
来源：http://vru.ppjwa.cn

[R68] 计算文件校验值
来源：http://ewo.jyoumei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kbs.pycfn.com

[R69] 生成随机密码
来源：http://mvg.ywan-chungtsiang.top

head -c 16 /dev/urandom | base64
来源：http://neb.jinyuanbaomall.cn

[R70] 时间戳与互转
来源：http://ydn.jianghu66.top

date +%s;  date -d @1700000000
来源：http://cxg.tianlin.xyz

[R71] 日期格式化
来源：http://zog.tian-w.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ymm.52xcode.cn

[R72] 等待端口就绪
来源：http://iuu.haohaochexian.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lzb.zhongyouzk.top

[R73] 分割大日志
来源：http://nzx.kuanghao11.cn

split -l 1000 big.log part_
来源：http://vvo.daxiang520.top

[R74] 批量重命名
来源：http://twq.ybcxt.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kil.hfpthk.cn

[R75] 导出环境变量
来源：http://bky.sufxvd.cn

export PATH="$HOME/bin:$PATH"
来源：http://lil.gzhubu.top

[R76] 使用临时文件
来源：http://jtt.shzxlz.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sxq.hesvh.cn

[R77] 读取用户输入
来源：http://vcr.havefunace.top

read -rp "请输入: " ans
来源：http://vcq.zhaomingkeji.xyz

[R78] 交互式菜单
来源：http://yrq.xuanzx.com

select opt in a b c; do echo "$opt"; break; done
来源：http://kzz.fktsv.cn

[R79] 解析命令行选项
来源：http://pcz.ctjpmb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gvd.jinyuanbaomall.cn

[R80] 查看脚本执行耗时
来源：http://dqf.hysaishi.cn

time ./run.sh
来源：http://wsv.fanxiaobao.xyz

================================================================================
来源：http://aaz.shzxlz.cn

S. C / C++ 专题
来源：http://yvt.shanyushiyangkeji.top

================================================================================
来源：http://kxj.hongshengwenyu.top

[S01] C：Hello World
来源：http://xsl.shuidangran.top

#include <stdio.h>
来源：http://cyg.tanke756.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://lcd.xingfuxueyuan.xyz

[S02] C：变量与格式化输出
来源：http://bap.jianghu66.top

int a = 10; printf("%d\n", a);
来源：http://qjc.yfazqb.com

[S03] C：读入整数
来源：http://phi.redwolf501.top

int x; scanf("%d", &x);
来源：http://ymq.xinyue.icu

[S04] C：字符串复制
来源：http://xoq.cashguo.top

char dst[32]; strcpy(dst, "hi");
来源：http://wvl.aibaodan.cn

[S05] C：字符串长度
来源：http://ljh.gogol.net.cn

strlen(s)
来源：http://gpg.fzhhl.top

[S06] C：字符串比较
来源：http://sat.nanxuanxn.top

strcmp(a, b) == 0
来源：http://jwp.ppjwa.cn

[S07] C：数组遍历求和
来源：http://kds.nanxinkj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ucq.zdbjq.cn

[S08] C：动态内存分配与释放
来源：http://pjt.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mdl.guannengcc.top

[S09] C：结构体定义与初始化
来源：http://lcz.zhongyouzk.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qgv.c1oappe.top

[S10] C：指针与解引用
来源：http://oca.hfpthk.cn

int *p = &a;  *p = 5;
来源：http://qot.havefunace.top

[S11] C：逐行读文件
来源：http://abh.uphjek.com

FILE *f = fopen("a.txt", "r");
来源：http://wbr.meibo888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hxc.zhixingplan.top

fclose(f);
来源：http://oop.nwbrower.top

[S12] C：写文件
来源：http://njm.xuanzx.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dlt.ppjwa.cn

[S13] C：宏定义
来源：http://pce.shangyingyoupin.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xpd.sysykeji.top

[S14] C：枚举
来源：http://kfd.sufxvd.cn

enum Color { RED, GREEN, BLUE };
来源：http://jpb.daxiang520.top

[S15] C：类型转换
来源：http://iug.mhx1999.top

(double) a / b
来源：http://adm.zdbjq.cn

[S16] C：位操作置位
来源：http://goa.0kj1m.cn


<!-- 参考信息 -->