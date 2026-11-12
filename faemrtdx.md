代发 wailian999

[Q48] CTE 公用表表达式
来源：http://emd.hysaishi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kwl.svipenyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://djy.daria6918.cn

[Q49] 更新单行
来源：http://jai.shanyushiyangtech.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cxe.uphjek.com

[Q50] 批量更新
来源：http://dmm.52xcode.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yhw.uphjek.com

[Q51] 用子查询更新
来源：http://ggf.jinqigfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qey.fengsongda.top

[Q52] 删除指定行
来源：http://hqy.aizwys.cn

DELETE FROM users WHERE id = 10;
来源：http://meo.nanxuanxn.top

[Q53] 按条件删除
来源：http://adr.guannengcc.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uaj.zdqjudy.top

[Q54] 清空表
来源：http://rio.gzhubu.top

TRUNCATE TABLE logs;
来源：http://rgf.316326.xyz

[Q55] 排名（并列占位）
来源：http://qsn.meibo888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tcz.yj202588.top

[Q56] 密集排名（并列不占位）
来源：http://ahj.aizwys.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tao.hfpthk.cn

[Q57] 行号
来源：http://fui.hnxiangtu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hrb.tian-w.cn

[Q58] 累计求和
来源：http://yjw.chenlongwang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rcv.gotoacloud.top

[Q59] 分组内累计
来源：http://zgi.jianghu66.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kyg.jqgfzy.top

[Q60] 取上一行 / 下一行
来源：http://scv.daxiang520.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ieq.ppjwa.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vti.mhx1999.top

[Q61] 移动平均
来源：http://tod.nanxuanxn.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mpd.dashuyun.cn

[Q62] 分组占比
来源：http://hek.cdnleiting.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://owx.ydzc1.top

[Q63] 开启事务
来源：http://krg.gaohongyu789.top

START TRANSACTION;                -- 或 BEGIN
来源：http://uah.gaohongyu789.top

[Q64] 提交事务
来源：http://msz.9152youxi.cn

COMMIT;
来源：http://wls.zhijiandao.cn

[Q65] 回滚事务
来源：http://fue.daria6918.cn

ROLLBACK;
来源：http://jhv.jiagoushi.top

[Q66] 行锁查询
来源：http://nxk.tarul.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lnw.ctjpmb.com

[Q67] 设置隔离级别
来源：http://dng.shangyingyoupin.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nrh.redwolf501.top

[Q68] 保存点
来源：http://kag.ywan-chungtsiang.top

SAVEPOINT sp1;
来源：http://lau.yj202588.top

ROLLBACK TO sp1;
来源：http://xaq.tianlin.xyz

[Q69] 查看执行计划
来源：http://eev.zdqjudy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ygv.andypj.xyz

[Q70] 更新统计信息
来源：http://lzs.svipenyu.cn

ANALYZE TABLE users;
来源：http://enu.jqgufenzy.top

[Q71] 查看建表语句
来源：http://kwb.hysaishi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gjk.bbcook.cn

[Q72] 查看索引
来源：http://rub.zdbjq.cn

SHOW INDEX FROM users;
来源：http://bpv.sjlbkw.cn

[Q73] 查看表状态
来源：http://vwm.dashuyun.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pub.snrcjt.cn

[Q74] 强制使用索引
来源：http://noc.jinqigufen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fxv.jinghuilouyu.cn

[Q75] 日期格式化
来源：http://rtp.smart0.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jzi.vehdjk.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hle.daria6918.cn

[Q76] 按天统计
来源：http://hyq.smart0.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lmw.shzxlz.cn

[Q77] 时间加减
来源：http://rgu.hfpthk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://opl.epnwcf.com

[Q78] 当前时间
来源：http://wvz.shzxlz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bwe.yuxming.cn

[Q79] 字符串拼接
来源：http://dtr.andypj.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tte.guowangkeji.top

[Q80] 字符串截取
来源：http://uhr.gzhubu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://raa.0kj1m.cn

[Q81] 字符串替换
来源：http://zah.sjlbkw.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yte.daxiang520.top

[Q82] 字符长度与字节长度
来源：http://rml.zhiwuduotai.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ljg.jinyuanbaomall.cn

[Q83] 大小写转换
来源：http://tol.birdmap.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bqk.redwolf501.top

[Q84] 去除首尾空格
来源：http://ibp.shanyushiyangtech.top

SELECT TRIM(name) FROM users;
来源：http://bso.vqdsnc.cn

[Q85] 数值取整
来源：http://dkt.yongpay.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zes.xinyue.icu

[Q86] 读取 JSON 字段
来源：http://ggd.c1oappe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dyh.zhengqikj.top

[Q87] JSON 字段做条件
来源：http://qto.hammf.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rnq.epnwcf.com

[Q88] 行转列（条件聚合）
来源：http://dfe.ywan-chungtsiang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tpm.guowangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://klz.cdnleiting.top

[Q89] 判断表是否存在
来源：http://zwi.hnqzz.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gox.jianghu66.top

[Q90] 生成序号列
来源：http://hvh.yongpay.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lir.hammf.cn

================================================================================
来源：http://toc.jianghu66.top

R. Bash 专题
来源：http://fmx.tianlin.xyz

================================================================================
来源：http://fib.uphjek.com

[R01] shebang 与严格模式
来源：http://vsp.meibo888.top

#!/usr/bin/env bash
来源：http://tqz.iojbl.cn

set -euo pipefail
来源：http://pos.yueranfly.top

[R02] 变量赋值与使用
来源：http://kyv.birdmap.top

name="Tom"; echo "$name"
来源：http://oug.jyoumei.cn

[R03] 只读变量
来源：http://mpe.nanxinkj.top

readonly PI=3.14
来源：http://sjs.cheryme.top

[R04] 位置参数
来源：http://imq.zhengqikj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://izy.mhx1999.top

[R05] 参数默认值
来源：http://ldx.feifeiyinyue.top

name="${1:-default}"
来源：http://xdn.fengsongda.top

[R06] 判断命令是否存在
来源：http://cbf.yueranfly.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cmz.c1oappe.top

[R07] if 判断文件
来源：http://zhv.ybcxt.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cxp.sysykeji.top

[R08] 数值比较
来源：http://myf.hnqzz.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zrc.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://uxj.xylfe.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wmw.zhoulong.xyz

[R10] 正则匹配
来源：http://bib.gotoacloud.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gbj.fzhhl.top

[R11] case 多分支
来源：http://bxm.zdqjudy.top

case "$1" in
来源：http://mhc.yj20258.top

start) echo "启动" ;;
来源：http://klm.zhijiandao.cn

stop)  echo "停止" ;;
来源：http://zun.bjfxy.top

*)     echo "未知命令" ;;
来源：http://qnz.jiagoushi.top

esac
来源：http://ztj.jyoumei.cn

[R12] for 遍历文件
来源：http://afe.jianghu66.top

for f in *.txt; do echo "$f"; done
来源：http://pgc.ydzc1.top

[R13] for 计数循环
来源：http://fvj.hammf.cn

for i in {1..10}; do echo "$i"; done
来源：http://txh.shanyushiyangkeji.top

[R14] C 风格 for
来源：http://vnt.yanxiufei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tmg.aizwys.cn

[R15] while 逐行读文件
来源：http://rmu.bjfxy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pmt.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://lsm.jqgfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xxy.zhengqikj.top

[R17] 数组定义与取值
来源：http://qnv.cucudq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ndm.ydzc1.top

[R18] 遍历数组
来源：http://jxc.xylfe.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xfv.gotoacloud.top

[R19] 数组长度
来源：http://ufp.tanke756.top

echo "${#arr[@]}"
来源：http://qmm.xinyue.icu

[R20] 关联数组（字典）
来源：http://hcw.yfazqb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zgv.hammf.cn

[R21] 字符串长度
来源：http://kxs.snrcjt.cn

echo "${#s}"
来源：http://zkp.epnwcf.com

[R22] 截取子串
来源：http://urm.yvedp.cn

echo "${s:0:5}"
来源：http://prs.yuanzhike.top

[R23] 字符串替换
来源：http://fpj.yvedp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vcu.vehdjk.com

[R24] 大小写转换
来源：http://ysu.birdmap.top

echo "${s^^}"; echo "${s,,}"
来源：http://mge.quarkkingdee.top

[R25] 去后缀 / 去前缀
来源：http://fmp.yj20258888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://odu.sysykeji.top

[R26] 命令替换
来源：http://utg.fehbvm.com

now=$(date +%F); echo "$now"
来源：http://yjo.mhx1999.top

[R27] 算术展开
来源：http://zeh.gogol.net.cn

echo $((1 + 2 * 3))
来源：http://vfa.vqdsnc.cn

[R28] 浮点运算
来源：http://dnw.cashguo.top

echo "scale=2; 10/3" | bc
来源：http://keo.fktsv.cn

[R29] 定义函数
来源：http://hxy.haohaochexian.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ocp.chenzaomai.com

[R30] 函数返回状态码
来源：http://zup.yj202588.top

f() { return 0; }; f || echo "失败了"
来源：http://ttw.ctjpmb.com

[R31] 局部变量
来源：http://rfo.yongpay.top

f() { local x=1; echo "$x"; }
来源：http://tto.jinyuanbaomall.cn

[R32] 参数个数校验
来源：http://igy.wangdashe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ypl.haohaochexian.top

[R33] 捕获错误并提示行号
来源：http://fsc.tarul.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zas.daria6918.cn

[R34] 退出时清理
来源：http://wbr.zhiwuduotai.top

trap 'rm -f "$tmp"' EXIT
来源：http://bny.epnwcf.com

[R35] 后台执行并等待
来源：http://snq.pycfn.com

sleep 5 & pid=$!; wait "$pid"
来源：http://qmn.xingfuxueyuan.xyz

[R36] 并发执行多个任务
来源：http://csa.yuxming.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hox.quarkkingdee.top

[R37] 把输出赋给变量
来源：http://zup.fzhhl.top

files=$(ls -1)
来源：http://anw.zdqjudy.top

[R38] 管道串联
来源：http://klg.hcnkem.com

cat a.txt | grep -i error | wc -l
来源：http://ynw.sysykeji.top

[R39] 重定向标准输出与错误
来源：http://hxd.ydjk.org.cn

cmd > out.log 2>&1
来源：http://yih.guannengcc.top

[R40] 追加写日志
来源：http://cbj.ppjwa.cn

echo "log" >> out.log
来源：http://nwp.ybcxt.top

[R41] 丢弃输出
来源：http://kwn.jinghuilouyu.cn

cmd >/dev/null 2>&1
来源：http://oci.redwolf501.top

[R42] 输入重定向
来源：http://gla.meibo888.top

wc -l < a.txt
来源：http://noa.fzhhl.top

[R43] 按名字查找文件
来源：http://dca.hnxiangtu.top

find . -name "*.log" -type f
来源：http://ery.ctjpmb.com

[R44] 按修改时间查找
来源：http://yuj.birdmap.top

find . -mtime -7 -type f
来源：http://prk.yj202588.top

[R45] 批量删除
来源：http://eqt.xingfuxueyuan.xyz

find . -name "*.tmp" -delete
来源：http://ihh.vehdjk.com

[R46] 递归替换文件内容
来源：http://rla.sweek.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rat.sysykeji.top

[R47] sed 单行替换
来源：http://yib.cqqwz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dcf.jlsjyb.cn

[R48] awk 取指定列
来源：http://xwk.xingfuxueyuan.xyz

awk '{print $1, $3}' a.txt
来源：http://ity.jinghuilouyu.cn

[R49] awk 带条件
来源：http://iad.cashguo.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pol.daxiang520.top

[R50] awk 求和
来源：http://hcx.tarul.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fst.yfazqb.com

[R51] 排序去重取前几
来源：http://lrr.yj20258888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bkd.cucudq.cn

[R52] 统计行数
来源：http://zpe.nanxuanxn.top

wc -l a.txt
来源：http://hiv.nwbrower.top

[R53] 查看文件头与实时尾
来源：http://kry.vehdjk.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fye.hcnkem.com

[R54] 比较两个文件
来源：http://kln.chenjidiqi.icu

diff a.txt b.txt
来源：http://iyh.nwbrower.top

[R55] 压缩与解压
来源：http://gqt.hywenlv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ydg.gogol.net.cn

[R56] 远程拷贝
来源：http://uxk.c1oappe.top

scp file user@host:/path/
来源：http://wqx.jinqigfzy.top

[R57] 远程执行命令
来源：http://jlg.tanke756.top

ssh user@host 'uptime'
来源：http://dmg.zhijiandao.cn

[R58] 下载文件
来源：http://cvj.zhijiandao.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wzs.shanyushiyangtech.top

[R59] 发 POST JSON
来源：http://dze.cheryme.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rnc.guannengcc.top

[R60] 只看 HTTP 状态码
来源：http://vdu.ehwqpu.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://byj.hfpthk.cn

[R61] 磁盘占用
来源：http://twj.daxiang520.top

df -h;  du -sh *
来源：http://seb.jinqigufen.top

[R62] 找最占空间的文件
来源：http://yzb.sweek.top

du -ah . | sort -rh | head -10
来源：http://hrn.jqgufenzy.top

[R63] 内存与进程
来源：http://hul.aizwys.cn

free -h;  ps aux | grep nginx
来源：http://cza.yanxiufei.cn

[R64] 结束进程
来源：http://vqy.hysaishi.cn

kill -9 $(pgrep -f app.py)
来源：http://sky.zhiwuduotai.top

[R65] 查看端口占用
来源：http://lpp.chenlongwang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pwq.fanxiaobao.xyz

[R66] 定时任务
来源：http://aql.yongpay.top

crontab -e;  crontab -l
来源：http://mbp.redwolf501.top

[R67] 生成随机十六进制串
来源：http://ifd.yonumen.top

openssl rand -hex 16
来源：http://obt.ybcxt.top

[R68] 计算文件校验值
来源：http://rmw.ywan-chungtsiang.top

sha256sum a.txt;  md5sum a.txt
来源：http://cpw.yj202588.top

[R69] 生成随机密码
来源：http://gdr.xinyue.icu

head -c 16 /dev/urandom | base64
来源：http://zbe.zhoulong.xyz

[R70] 时间戳与互转
来源：http://frh.yuanzhike.top

date +%s;  date -d @1700000000
来源：http://lky.jqgufenzy.top

[R71] 日期格式化
来源：http://zes.kuanghao11.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jgh.shangyingyoupin.top

[R72] 等待端口就绪
来源：http://ifg.cashguo.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mwd.nanxinkj.top

[R73] 分割大日志
来源：http://xzd.dianchejie.cn

split -l 1000 big.log part_
来源：http://xpj.hnqzz.top

[R74] 批量重命名
来源：http://lly.zhoulong.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pzo.aizwys.cn

[R75] 导出环境变量
来源：http://ygh.chenjidiqi.icu

export PATH="$HOME/bin:$PATH"
来源：http://aqi.jyoumei.cn

[R76] 使用临时文件
来源：http://vxa.vehdjk.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qtt.hammf.cn

[R77] 读取用户输入
来源：http://rsm.c1oappe.top

read -rp "请输入: " ans
来源：http://tzd.smart0.xyz

[R78] 交互式菜单
来源：http://uyr.xylfe.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cli.hcnkem.com

[R79] 解析命令行选项
来源：http://okc.zhengqikj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lys.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://ikk.hnqzz.top

time ./run.sh
来源：http://six.yueranfly.top

================================================================================
来源：http://vhl.gaohongyu789.top

S. C / C++ 专题
来源：http://agz.zhongyouzk.top

================================================================================
来源：http://vlt.epnwcf.com

[S01] C：Hello World
来源：http://xzc.jinqigufen.top

#include <stdio.h>
来源：http://oik.fengsongda.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ztb.dianchejie.cn

[S02] C：变量与格式化输出
来源：http://tsg.wangdashe.top

int a = 10; printf("%d\n", a);
来源：http://bwa.nanxuanxn.top

[S03] C：读入整数
来源：http://wlm.svipenyu.cn

int x; scanf("%d", &x);
来源：http://vxn.dashuyun.cn

[S04] C：字符串复制
来源：http://xsc.ydjk.org.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zqg.bjfxy.top

[S05] C：字符串长度
来源：http://pbm.shangyingyoupin.top

strlen(s)
来源：http://sxq.yfazqb.com

[S06] C：字符串比较
来源：http://ebd.0kj1m.cn

strcmp(a, b) == 0
来源：http://kjo.wangshuangyany.cn

[S07] C：数组遍历求和
来源：http://fsw.nanxinkj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ixg.hnxiangtu.top

[S08] C：动态内存分配与释放
来源：http://ygu.ehwqpu.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ccy.nwbrower.top

[S09] C：结构体定义与初始化
来源：http://iao.gaohongyu789.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jyk.sweek.top

[S10] C：指针与解引用
来源：http://kmt.xylfe.cn

int *p = &a;  *p = 5;
来源：http://avp.yfazqb.com

[S11] C：逐行读文件
来源：http://xlo.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://zxs.yuxming.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://plv.quarkkingdee.top

fclose(f);
来源：http://mzn.zhoulong.xyz

[S12] C：写文件
来源：http://qgq.pycfn.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vcw.guannengcc.top

[S13] C：宏定义
来源：http://wsk.ywan-chungtsiang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eex.jinghuilouyu.cn

[S14] C：枚举
来源：http://stk.fanxiaobao.xyz

enum Color { RED, GREEN, BLUE };
来源：http://onz.sufxvd.cn

[S15] C：类型转换
来源：http://hzf.snrcjt.cn

(double) a / b
来源：http://dqk.gzhubu.top

[S16] C：位操作置位
来源：http://tmm.yj202588.top

x |= (1 << 3);
来源：http://ump.haohaochexian.top

[S17] C：安全拼接字符串
来源：http://fti.fengsongda.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ftv.iojbl.cn

[S18] C：命令行参数
来源：http://ias.jqgfzy.top


<!-- 参考信息 -->