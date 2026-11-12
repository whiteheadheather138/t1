代发 wailian999

[Q48] CTE 公用表表达式
来源：http://gpo.316326.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cnw.zhongyouzk.top

SELECT * FROM t WHERE c > 5;
来源：http://eol.quarkkingdee.top

[Q49] 更新单行
来源：http://ydx.xziqi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ddk.hnxiangtu.top

[Q50] 批量更新
来源：http://blk.hysaishi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jxc.wangdashe.top

[Q51] 用子查询更新
来源：http://fld.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vgs.xingfuxueyuan.xyz

[Q52] 删除指定行
来源：http://hku.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://uam.yonumen.top

[Q53] 按条件删除
来源：http://zly.ehwqpu.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hkn.fktsv.cn

[Q54] 清空表
来源：http://vfr.tanke756.top

TRUNCATE TABLE logs;
来源：http://gib.xuanzx.com

[Q55] 排名（并列占位）
来源：http://sqf.feifeiyinyue.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://phj.sysykeji.top

[Q56] 密集排名（并列不占位）
来源：http://twx.iojbl.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wdg.bjfxy.top

[Q57] 行号
来源：http://zzb.haohaochexian.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wxo.ydzc1.top

[Q58] 累计求和
来源：http://its.jinqigfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zss.fzhhl.top

[Q59] 分组内累计
来源：http://wys.fengsongda.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ybk.xinyue.icu

[Q60] 取上一行 / 下一行
来源：http://quf.yonumen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ttm.shanyushiyangtech.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://epw.jinghuilouyu.cn

[Q61] 移动平均
来源：http://fuu.yanxiufei.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://inz.ehwqpu.com

[Q62] 分组占比
来源：http://pxo.yangfankeji.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yey.jyoumei.cn

[Q63] 开启事务
来源：http://qui.sjlbkw.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://imb.svipenyu.cn

[Q64] 提交事务
来源：http://lyz.mhx1999.top

COMMIT;
来源：http://plj.aibaodan.cn

[Q65] 回滚事务
来源：http://qct.shanyushiyangtech.top

ROLLBACK;
来源：http://hwy.zhengqikj.top

[Q66] 行锁查询
来源：http://lsl.aizwys.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dbv.zdqjudy.top

[Q67] 设置隔离级别
来源：http://sby.nwbrower.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zbo.ctjpmb.com

[Q68] 保存点
来源：http://alw.ydzc1.top

SAVEPOINT sp1;
来源：http://nzg.tarul.cn

ROLLBACK TO sp1;
来源：http://ymc.yuanzhike.top

[Q69] 查看执行计划
来源：http://spr.tanke756.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dlp.gaohongyu789.top

[Q70] 更新统计信息
来源：http://isp.0kj1m.cn

ANALYZE TABLE users;
来源：http://fyz.ehwqpu.com

[Q71] 查看建表语句
来源：http://ryr.ybcxt.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kcv.hnqzz.top

[Q72] 查看索引
来源：http://sry.yj20258.top

SHOW INDEX FROM users;
来源：http://bag.yuanzhike.top

[Q73] 查看表状态
来源：http://xwk.daxiang520.top

SHOW TABLE STATUS LIKE 'users';
来源：http://scw.cashguo.top

[Q74] 强制使用索引
来源：http://vwt.zhoulong.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qxd.jinqigufen.top

[Q75] 日期格式化
来源：http://isj.chenjidiqi.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fcw.svipenyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tvd.sxryk.cn

[Q76] 按天统计
来源：http://inp.andypj.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yxg.fehbvm.com

[Q77] 时间加减
来源：http://rqh.birdmap.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://evr.gzhubu.top

[Q78] 当前时间
来源：http://oav.xylfe.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oow.shzxlz.cn

[Q79] 字符串拼接
来源：http://cgp.hcnkem.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yws.jyoumei.cn

[Q80] 字符串截取
来源：http://hkw.cucudq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oxv.hongshengwenyu.top

[Q81] 字符串替换
来源：http://cqc.vqdsnc.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gry.hcnkem.com

[Q82] 字符长度与字节长度
来源：http://zic.yongpay.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://smc.tianlin.xyz

[Q83] 大小写转换
来源：http://rft.tianlin.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mcg.fanxiaobao.xyz

[Q84] 去除首尾空格
来源：http://jdz.shanyushiyangkeji.top

SELECT TRIM(name) FROM users;
来源：http://oze.hcnkem.com

[Q85] 数值取整
来源：http://hno.pengpengdd.cyou

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xif.zhengqikj.top

[Q86] 读取 JSON 字段
来源：http://dji.shanyushiyangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qqs.nwbrower.top

[Q87] JSON 字段做条件
来源：http://qwl.ivvv.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rkg.wangdashe.top

[Q88] 行转列（条件聚合）
来源：http://ing.xingfuxueyuan.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sda.uphjek.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pnd.dianchejie.cn

[Q89] 判断表是否存在
来源：http://jsu.zdqjudy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pjl.ehwqpu.com

[Q90] 生成序号列
来源：http://fvh.tianlin.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://haw.bbcook.cn

================================================================================
来源：http://eea.xziqi.cn

R. Bash 专题
来源：http://xby.fehbvm.com

================================================================================
来源：http://cad.shanyushiyangkeji.top

[R01] shebang 与严格模式
来源：http://ikd.zycfv.cn

#!/usr/bin/env bash
来源：http://xov.tian-w.cn

set -euo pipefail
来源：http://snb.mhx1999.top

[R02] 变量赋值与使用
来源：http://vdm.yfazqb.com

name="Tom"; echo "$name"
来源：http://fic.quarkkingdee.top

[R03] 只读变量
来源：http://gjc.yj20258888.top

readonly PI=3.14
来源：http://xnx.fzhhl.top

[R04] 位置参数
来源：http://czl.jinqigfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ldr.vehdjk.com

[R05] 参数默认值
来源：http://mij.hesvh.cn

name="${1:-default}"
来源：http://eqk.hcnkem.com

[R06] 判断命令是否存在
来源：http://nle.uphjek.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://egi.hnqzz.top

[R07] if 判断文件
来源：http://rvi.zhijiandao.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://des.daxiang520.top

[R08] 数值比较
来源：http://yeh.dianchejie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://aym.ybcxt.top

[R09] 字符串比较
来源：http://onv.fktsv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rwp.gzhubu.top

[R10] 正则匹配
来源：http://nlp.yj20258888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ogz.shanyushiyangtech.top

[R11] case 多分支
来源：http://hvm.hywenlv.cn

case "$1" in
来源：http://ywj.haohaochexian.top

start) echo "启动" ;;
来源：http://oqp.pengpengdd.cyou

stop)  echo "停止" ;;
来源：http://mmv.guowangkeji.top

*)     echo "未知命令" ;;
来源：http://tbt.ybcxt.top

esac
来源：http://ctc.jyoumei.cn

[R12] for 遍历文件
来源：http://fky.shzxlz.cn

for f in *.txt; do echo "$f"; done
来源：http://jom.bjfxy.top

[R13] for 计数循环
来源：http://vzb.fengsongda.top

for i in {1..10}; do echo "$i"; done
来源：http://oin.ywan-chungtsiang.top

[R14] C 风格 for
来源：http://das.jinqigufen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dpz.yueranfly.top

[R15] while 逐行读文件
来源：http://qif.dianchejie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rol.yanxiufei.cn

[R16] until 等待条件
来源：http://exy.gotoacloud.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://try.ehwqpu.com

[R17] 数组定义与取值
来源：http://glm.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ejx.jqgufenzy.top

[R18] 遍历数组
来源：http://wkf.ctjpmb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xkp.jyoumei.cn

[R19] 数组长度
来源：http://odz.dianchejie.cn

echo "${#arr[@]}"
来源：http://lix.nanxinkj.top

[R20] 关联数组（字典）
来源：http://xcu.yfazqb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zzb.quarkkingdee.top

[R21] 字符串长度
来源：http://ytk.ydjk.org.cn

echo "${#s}"
来源：http://qaa.wangshuangyany.cn

[R22] 截取子串
来源：http://yfb.jlsjyb.cn

echo "${s:0:5}"
来源：http://gaf.havefunace.top

[R23] 字符串替换
来源：http://pdh.jinqigufen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jsc.fktsv.cn

[R24] 大小写转换
来源：http://msg.9152youxi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zxk.aizwys.cn

[R25] 去后缀 / 去前缀
来源：http://brw.chenlongwang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://oyc.xuanzx.com

[R26] 命令替换
来源：http://zvr.wangshuangyany.cn

now=$(date +%F); echo "$now"
来源：http://dqr.gotoacloud.top

[R27] 算术展开
来源：http://flr.dashuyun.cn

echo $((1 + 2 * 3))
来源：http://zbo.shanyushiyangtech.top

[R28] 浮点运算
来源：http://sge.52xcode.cn

echo "scale=2; 10/3" | bc
来源：http://nui.sweek.top

[R29] 定义函数
来源：http://tvj.9152youxi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dqv.nanxuanxn.top

[R30] 函数返回状态码
来源：http://lmi.daxiang520.top

f() { return 0; }; f || echo "失败了"
来源：http://crw.epnwcf.com

[R31] 局部变量
来源：http://upd.andypj.xyz

f() { local x=1; echo "$x"; }
来源：http://lsm.ydjk.org.cn

[R32] 参数个数校验
来源：http://uwe.jqgfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://peo.yangfankeji.com

[R33] 捕获错误并提示行号
来源：http://urw.hcnkem.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lyp.jinqigfzy.top

[R34] 退出时清理
来源：http://bgf.epnwcf.com

trap 'rm -f "$tmp"' EXIT
来源：http://lxo.yuanzhike.top

[R35] 后台执行并等待
来源：http://gwq.andypj.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://uqf.zhijiandao.cn

[R36] 并发执行多个任务
来源：http://gaj.ydzc1.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xar.zhengqikj.top

[R37] 把输出赋给变量
来源：http://ohz.quarkkingdee.top

files=$(ls -1)
来源：http://ciq.bbcook.cn

[R38] 管道串联
来源：http://qag.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://erx.xingfuxueyuan.xyz

[R39] 重定向标准输出与错误
来源：http://uea.zhijiandao.cn

cmd > out.log 2>&1
来源：http://ynl.cashguo.top

[R40] 追加写日志
来源：http://ocp.daria6918.cn

echo "log" >> out.log
来源：http://ixs.yangfankeji.com

[R41] 丢弃输出
来源：http://fqf.birdmap.top

cmd >/dev/null 2>&1
来源：http://jbr.cqqwz.cn

[R42] 输入重定向
来源：http://nuf.zhijiandao.cn

wc -l < a.txt
来源：http://cav.xingfuxueyuan.xyz

[R43] 按名字查找文件
来源：http://oih.zdbjq.cn

find . -name "*.log" -type f
来源：http://fjm.tarul.cn

[R44] 按修改时间查找
来源：http://zdi.tanke756.top

find . -mtime -7 -type f
来源：http://eax.cqqwz.cn

[R45] 批量删除
来源：http://wpn.ctjpmb.com

find . -name "*.tmp" -delete
来源：http://nmb.hammf.cn

[R46] 递归替换文件内容
来源：http://lsw.snrcjt.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ihd.aizwys.cn

[R47] sed 单行替换
来源：http://iwo.yj202588.top

sed -i 's/foo/bar/g' a.txt
来源：http://hnk.jinyuanbaomall.cn

[R48] awk 取指定列
来源：http://ytp.bjfxy.top

awk '{print $1, $3}' a.txt
来源：http://hgu.shangyingyoupin.top

[R49] awk 带条件
来源：http://kdg.zhoulong.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vlj.guowangkeji.top

[R50] awk 求和
来源：http://yko.hcnkem.com

awk '{s += $2} END {print s}' a.txt
来源：http://pja.zycfv.cn

[R51] 排序去重取前几
来源：http://nps.pycfn.com

sort a.txt | uniq -c | sort -rn | head
来源：http://syy.xinyue.icu

[R52] 统计行数
来源：http://uqd.cashguo.top

wc -l a.txt
来源：http://wpt.vehdjk.com

[R53] 查看文件头与实时尾
来源：http://pqj.ppjwa.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zoz.sjlbkw.cn

[R54] 比较两个文件
来源：http://usp.hnqzz.top

diff a.txt b.txt
来源：http://wpr.birdmap.top

[R55] 压缩与解压
来源：http://qgj.ydjk.org.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://idz.hnqzz.top

[R56] 远程拷贝
来源：http://qee.yangfankeji.com

scp file user@host:/path/
来源：http://ljr.aizwys.cn

[R57] 远程执行命令
来源：http://udl.cheryme.top

ssh user@host 'uptime'
来源：http://ksh.tian-w.cn

[R58] 下载文件
来源：http://udk.yj202588.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xlp.gotoacloud.top

[R59] 发 POST JSON
来源：http://cid.hesvh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dog.hnqzz.top

[R60] 只看 HTTP 状态码
来源：http://glj.shanyushiyangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://paz.hywenlv.cn

[R61] 磁盘占用
来源：http://acv.havefunace.top

df -h;  du -sh *
来源：http://hif.chenlongwang.top

[R62] 找最占空间的文件
来源：http://kaw.sjlbkw.cn

du -ah . | sort -rh | head -10
来源：http://uir.cucudq.cn

[R63] 内存与进程
来源：http://obw.wangshuangyany.cn

free -h;  ps aux | grep nginx
来源：http://fpc.yueranfly.top

[R64] 结束进程
来源：http://nmp.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://kac.havefunace.top

[R65] 查看端口占用
来源：http://ini.zhoulong.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jhq.yj202588.top

[R66] 定时任务
来源：http://nlo.gotoacloud.top

crontab -e;  crontab -l
来源：http://eyn.zhengqikj.top

[R67] 生成随机十六进制串
来源：http://pvs.tarul.cn

openssl rand -hex 16
来源：http://kgh.jqgfzy.top

[R68] 计算文件校验值
来源：http://cvr.nwbrower.top

sha256sum a.txt;  md5sum a.txt
来源：http://ejh.jyoumei.cn

[R69] 生成随机密码
来源：http://iwp.zhijiandao.cn

head -c 16 /dev/urandom | base64
来源：http://qkh.shuidangran.top

[R70] 时间戳与互转
来源：http://bhk.cheryme.top

date +%s;  date -d @1700000000
来源：http://vfw.ivvv.top

[R71] 日期格式化
来源：http://kkc.guannengcc.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lvd.316326.xyz

[R72] 等待端口就绪
来源：http://auo.wangshuangyany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://iit.chenlongwang.top

[R73] 分割大日志
来源：http://tfj.hcnkem.com

split -l 1000 big.log part_
来源：http://odu.shanyushiyangkeji.top

[R74] 批量重命名
来源：http://zxb.jqgufenzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aii.birdmap.top

[R75] 导出环境变量
来源：http://ddx.pycfn.com

export PATH="$HOME/bin:$PATH"
来源：http://hzv.sjlbkw.cn

[R76] 使用临时文件
来源：http://xco.iojbl.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rpp.tarul.cn

[R77] 读取用户输入
来源：http://aqw.ehwqpu.com

read -rp "请输入: " ans
来源：http://jyj.yueranfly.top

[R78] 交互式菜单
来源：http://llc.shanyushiyangtech.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wzb.hysaishi.cn

[R79] 解析命令行选项
来源：http://rnv.bbcook.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lhm.aizwys.cn

[R80] 查看脚本执行耗时
来源：http://aqo.bjfxy.top

time ./run.sh
来源：http://bjy.316326.xyz

================================================================================
来源：http://xno.cashguo.top

S. C / C++ 专题
来源：http://jey.zhijiandao.cn

================================================================================
来源：http://pvs.fktsv.cn

[S01] C：Hello World
来源：http://apm.zhixingplan.top

#include <stdio.h>
来源：http://rmx.yongpay.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ujv.zhaomingkeji.xyz

[S02] C：变量与格式化输出
来源：http://vbj.zhaomingkeji.xyz

int a = 10; printf("%d\n", a);
来源：http://vya.uphjek.com

[S03] C：读入整数
来源：http://kqw.zhoulong.xyz

int x; scanf("%d", &x);
来源：http://var.shanyushiyangtech.top

[S04] C：字符串复制
来源：http://ehj.hysaishi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://znu.aibaodan.cn

[S05] C：字符串长度
来源：http://gys.yongpay.top

strlen(s)
来源：http://qxj.ctjpmb.com

[S06] C：字符串比较
来源：http://nfl.zhiwuduotai.top

strcmp(a, b) == 0
来源：http://mjl.gaohongyu789.top

[S07] C：数组遍历求和
来源：http://ess.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://erd.chenlongwang.top

[S08] C：动态内存分配与释放
来源：http://sbp.epnwcf.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jig.jinghuilouyu.cn

[S09] C：结构体定义与初始化
来源：http://ruh.yongpay.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gou.hysaishi.cn

[S10] C：指针与解引用
来源：http://rzs.xziqi.cn

int *p = &a;  *p = 5;
来源：http://mvo.hywenlv.cn

[S11] C：逐行读文件
来源：http://pys.zhoulong.xyz

FILE *f = fopen("a.txt", "r");
来源：http://ydy.0kj1m.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hxp.yvedp.cn

fclose(f);
来源：http://ocs.fzhhl.top

[S12] C：写文件
来源：http://ncz.xuanzx.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uho.zdqjudy.top

[S13] C：宏定义
来源：http://yjc.ybcxt.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pcy.shanyushiyangkeji.top

[S14] C：枚举
来源：http://sjp.xuanzx.com

enum Color { RED, GREEN, BLUE };
来源：http://ajt.redwolf501.top

[S15] C：类型转换
来源：http://thy.yj20258888.top

(double) a / b
来源：http://cxn.ivvv.top

[S16] C：位操作置位
来源：http://fur.fktsv.cn

x |= (1 << 3);
来源：http://vso.havefunace.top

[S17] C：安全拼接字符串
来源：http://dew.ydjk.org.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kuu.jlsjyb.cn

[S18] C：命令行参数
来源：http://ymg.pycfn.com


<!-- 参考信息 -->