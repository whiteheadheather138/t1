代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cso.xylfe.cn

[Q56] 密集排名（并列不占位）
来源：http://ega.fehbvm.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://boj.yueranfly.top

[Q57] 行号
来源：http://owx.daria6918.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ltu.tarul.cn

[Q58] 累计求和
来源：http://gsc.wangshuangyany.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://req.dashuyun.cn

[Q59] 分组内累计
来源：http://vxl.chenjidiqi.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zar.sjlbkw.cn

[Q60] 取上一行 / 下一行
来源：http://zns.yongpay.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iqs.sjlbkw.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://apb.9152youxi.cn

[Q61] 移动平均
来源：http://mgf.mhx1999.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mdj.daxiang520.top

[Q62] 分组占比
来源：http://lqt.kuanghao11.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yzf.zhiwuduotai.top

[Q63] 开启事务
来源：http://mgn.smart0.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://uii.epnwcf.com

[Q64] 提交事务
来源：http://epw.nwbrower.top

COMMIT;
来源：http://aug.yj202588.top

[Q65] 回滚事务
来源：http://esi.shuidangran.top

ROLLBACK;
来源：http://dmi.havefunace.top

[Q66] 行锁查询
来源：http://hzc.hongshengwenyu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gkj.meibo888.top

[Q67] 设置隔离级别
来源：http://wbi.yanxiufei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tka.jqgfzy.top

[Q68] 保存点
来源：http://qnx.ydjk.org.cn

SAVEPOINT sp1;
来源：http://cxn.yuanzhike.top

ROLLBACK TO sp1;
来源：http://kxy.chenlongwang.top

[Q69] 查看执行计划
来源：http://byq.gogol.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uju.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://utg.gotoacloud.top

ANALYZE TABLE users;
来源：http://uml.fehbvm.com

[Q71] 查看建表语句
来源：http://vgw.sufxvd.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wqy.yvedp.cn

[Q72] 查看索引
来源：http://bjv.jinghuilouyu.cn

SHOW INDEX FROM users;
来源：http://svs.sysykeji.top

[Q73] 查看表状态
来源：http://nde.hnxiangtu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rmw.birdmap.top

[Q74] 强制使用索引
来源：http://qws.gogol.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jmt.zhengqikj.top

[Q75] 日期格式化
来源：http://kdy.nanxuanxn.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mok.zhengqikj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://prc.hysaishi.cn

[Q76] 按天统计
来源：http://umf.feifeiyinyue.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zsl.yfazqb.com

[Q77] 时间加减
来源：http://avp.xylfe.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eeq.andypj.xyz

[Q78] 当前时间
来源：http://sgf.zhiwuduotai.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lyf.hfpthk.cn

[Q79] 字符串拼接
来源：http://cuv.chenjidiqi.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zje.wangdashe.top

[Q80] 字符串截取
来源：http://bvc.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://egs.svipenyu.cn

[Q81] 字符串替换
来源：http://lys.hammf.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xhi.hywenlv.cn

[Q82] 字符长度与字节长度
来源：http://yni.meibo888.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kyx.gotoacloud.top

[Q83] 大小写转换
来源：http://gla.sysykeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xuv.feifeiyinyue.top

[Q84] 去除首尾空格
来源：http://alm.snrcjt.cn

SELECT TRIM(name) FROM users;
来源：http://vbu.hnqzz.top

[Q85] 数值取整
来源：http://fjj.yangfankeji.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jzg.shangyingyoupin.top

[Q86] 读取 JSON 字段
来源：http://cmr.jyoumei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sxo.ivvv.top

[Q87] JSON 字段做条件
来源：http://wyz.feifeiyinyue.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yoz.cashguo.top

[Q88] 行转列（条件聚合）
来源：http://nql.tianlin.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oqu.iojbl.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://npj.zhiwuduotai.top

[Q89] 判断表是否存在
来源：http://ucn.jinqigfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xbv.yongpay.top

[Q90] 生成序号列
来源：http://rrh.hywenlv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ivg.sufxvd.cn

================================================================================
来源：http://oxi.yongpay.top

R. Bash 专题
来源：http://mfi.ctjpmb.com

================================================================================
来源：http://kpb.gotoacloud.top

[R01] shebang 与严格模式
来源：http://uzk.aizwys.cn

#!/usr/bin/env bash
来源：http://abx.fengsongda.top

set -euo pipefail
来源：http://zcr.chenlongwang.top

[R02] 变量赋值与使用
来源：http://ziz.hywenlv.cn

name="Tom"; echo "$name"
来源：http://kob.jinqigfzy.top

[R03] 只读变量
来源：http://rpe.cqqwz.cn

readonly PI=3.14
来源：http://peh.shangyingyoupin.top

[R04] 位置参数
来源：http://zru.jiagoushi.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qum.0kj1m.cn

[R05] 参数默认值
来源：http://uvm.ywan-chungtsiang.top

name="${1:-default}"
来源：http://yrc.hfpthk.cn

[R06] 判断命令是否存在
来源：http://bzz.zhiwuduotai.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wfj.tarul.cn

[R07] if 判断文件
来源：http://tsc.hnxiangtu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sdq.smart0.xyz

[R08] 数值比较
来源：http://ced.jianghu66.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jax.shuidangran.top

[R09] 字符串比较
来源：http://lvz.iojbl.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://isn.xingfuxueyuan.xyz

[R10] 正则匹配
来源：http://rnq.xuanzx.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kpg.snrcjt.cn

[R11] case 多分支
来源：http://fyw.mhx1999.top

case "$1" in
来源：http://nqt.ydzc1.top

start) echo "启动" ;;
来源：http://ltj.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://dkm.c1oappe.top

*)     echo "未知命令" ;;
来源：http://pox.epnwcf.com

esac
来源：http://vpv.yfazqb.com

[R12] for 遍历文件
来源：http://rwk.mhx1999.top

for f in *.txt; do echo "$f"; done
来源：http://pee.jiagoushi.top

[R13] for 计数循环
来源：http://vtb.zhiwuduotai.top

for i in {1..10}; do echo "$i"; done
来源：http://mgy.zhengqikj.top

[R14] C 风格 for
来源：http://vqc.chenjidiqi.icu

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rtu.jqgufenzy.top

[R15] while 逐行读文件
来源：http://rfs.svipenyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://umq.fktsv.cn

[R16] until 等待条件
来源：http://hjr.shuidangran.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://enr.gotoacloud.top

[R17] 数组定义与取值
来源：http://cdv.epnwcf.com

arr=(a b c); echo "${arr[0]}"
来源：http://agq.iojbl.cn

[R18] 遍历数组
来源：http://sti.ydjk.org.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gvg.fanxiaobao.xyz

[R19] 数组长度
来源：http://iha.yfazqb.com

echo "${#arr[@]}"
来源：http://yex.cheryme.top

[R20] 关联数组（字典）
来源：http://uqx.sufxvd.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mgl.hfpthk.cn

[R21] 字符串长度
来源：http://iyo.aibaodan.cn

echo "${#s}"
来源：http://dyd.zhijiandao.cn

[R22] 截取子串
来源：http://cly.fehbvm.com

echo "${s:0:5}"
来源：http://wgp.0kj1m.cn

[R23] 字符串替换
来源：http://bry.redwolf501.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pxq.dianchejie.cn

[R24] 大小写转换
来源：http://qpt.hongshengwenyu.top

echo "${s^^}"; echo "${s,,}"
来源：http://uvf.sjlbkw.cn

[R25] 去后缀 / 去前缀
来源：http://fae.yj20258.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lci.feifeiyinyue.top

[R26] 命令替换
来源：http://rnt.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://drf.gogol.net.cn

[R27] 算术展开
来源：http://hjq.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://pro.jyoumei.cn

[R28] 浮点运算
来源：http://nmt.zhongyouzk.top

echo "scale=2; 10/3" | bc
来源：http://bjz.vqdsnc.cn

[R29] 定义函数
来源：http://ahz.guannengcc.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ieq.yanxiufei.cn

[R30] 函数返回状态码
来源：http://bpn.cashguo.top

f() { return 0; }; f || echo "失败了"
来源：http://swg.aibaodan.cn

[R31] 局部变量
来源：http://bqr.daxiang520.top

f() { local x=1; echo "$x"; }
来源：http://psb.gotoacloud.top

[R32] 参数个数校验
来源：http://xha.guowangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://chz.xingfuxueyuan.xyz

[R33] 捕获错误并提示行号
来源：http://yqq.meibo888.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://psb.hcnkem.com

[R34] 退出时清理
来源：http://lax.tanke756.top

trap 'rm -f "$tmp"' EXIT
来源：http://ilu.yonumen.top

[R35] 后台执行并等待
来源：http://orl.redwolf501.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bwr.hnxiangtu.top

[R36] 并发执行多个任务
来源：http://dcd.fzhhl.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mky.xylfe.cn

[R37] 把输出赋给变量
来源：http://vrf.zhiwuduotai.top

files=$(ls -1)
来源：http://xfv.chenlongwang.top

[R38] 管道串联
来源：http://ffp.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://umh.fzhhl.top

[R39] 重定向标准输出与错误
来源：http://tsi.gotoacloud.top

cmd > out.log 2>&1
来源：http://rco.daxiang520.top

[R40] 追加写日志
来源：http://fbe.mhx1999.top

echo "log" >> out.log
来源：http://trk.jlsjyb.cn

[R41] 丢弃输出
来源：http://rle.jiagoushi.top

cmd >/dev/null 2>&1
来源：http://uev.chenlongwang.top

[R42] 输入重定向
来源：http://ahf.hesvh.cn

wc -l < a.txt
来源：http://ius.xuanzx.com

[R43] 按名字查找文件
来源：http://ldp.vqdsnc.cn

find . -name "*.log" -type f
来源：http://jku.hnxiangtu.top

[R44] 按修改时间查找
来源：http://xva.tianlin.xyz

find . -mtime -7 -type f
来源：http://rqo.yangfankeji.com

[R45] 批量删除
来源：http://lub.ivvv.top

find . -name "*.tmp" -delete
来源：http://qts.pycfn.com

[R46] 递归替换文件内容
来源：http://ubp.zhongyouzk.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://btu.yj20258888.top

[R47] sed 单行替换
来源：http://jev.pengpengdd.cyou

sed -i 's/foo/bar/g' a.txt
来源：http://nid.zycfv.cn

[R48] awk 取指定列
来源：http://wzi.zhiwuduotai.top

awk '{print $1, $3}' a.txt
来源：http://fyf.ivvv.top

[R49] awk 带条件
来源：http://yop.haohaochexian.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wbx.jiagoushi.top

[R50] awk 求和
来源：http://kle.vqdsnc.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jca.mhx1999.top

[R51] 排序去重取前几
来源：http://egk.bbcook.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mad.haohaochexian.top

[R52] 统计行数
来源：http://kgx.fehbvm.com

wc -l a.txt
来源：http://vgc.gaohongyu789.top

[R53] 查看文件头与实时尾
来源：http://ntd.dianchejie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rtz.hesvh.cn

[R54] 比较两个文件
来源：http://pwy.iojbl.cn

diff a.txt b.txt
来源：http://gsx.yvedp.cn

[R55] 压缩与解压
来源：http://iuk.316326.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cry.hesvh.cn

[R56] 远程拷贝
来源：http://udz.pengpengdd.cyou

scp file user@host:/path/
来源：http://iew.wangshuangyany.cn

[R57] 远程执行命令
来源：http://yuu.zhoulong.xyz

ssh user@host 'uptime'
来源：http://bzv.yonumen.top

[R58] 下载文件
来源：http://epp.zhijiandao.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://afn.xinyue.icu

[R59] 发 POST JSON
来源：http://wrj.zhijiandao.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qpe.jqgfzy.top

[R60] 只看 HTTP 状态码
来源：http://lio.zdbjq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kts.hcnkem.com

[R61] 磁盘占用
来源：http://hdq.ydjk.org.cn

df -h;  du -sh *
来源：http://ghx.xuanzx.com

[R62] 找最占空间的文件
来源：http://tpm.zhaomingkeji.xyz

du -ah . | sort -rh | head -10
来源：http://clq.gzhubu.top

[R63] 内存与进程
来源：http://srx.ywan-chungtsiang.top

free -h;  ps aux | grep nginx
来源：http://ltb.wangdashe.top

[R64] 结束进程
来源：http://liu.hysaishi.cn

kill -9 $(pgrep -f app.py)
来源：http://ldi.pycfn.com

[R65] 查看端口占用
来源：http://zvy.yanxiufei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://chb.svipenyu.cn

[R66] 定时任务
来源：http://vvj.jinqigufen.top

crontab -e;  crontab -l
来源：http://dty.yj20258888.top

[R67] 生成随机十六进制串
来源：http://jqg.zhongyouzk.top

openssl rand -hex 16
来源：http://zrc.bbcook.cn

[R68] 计算文件校验值
来源：http://qxr.jinqigfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://vqi.vehdjk.com

[R69] 生成随机密码
来源：http://orr.hysaishi.cn

head -c 16 /dev/urandom | base64
来源：http://xjt.gotoacloud.top

[R70] 时间戳与互转
来源：http://dbz.tanke756.top

date +%s;  date -d @1700000000
来源：http://fln.iojbl.cn

[R71] 日期格式化
来源：http://fmg.tarul.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ole.yongpay.top

[R72] 等待端口就绪
来源：http://ros.feifeiyinyue.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yll.316326.xyz

[R73] 分割大日志
来源：http://kpv.jinqigfzy.top

split -l 1000 big.log part_
来源：http://yrx.zhongyouzk.top

[R74] 批量重命名
来源：http://nxg.shuidangran.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bip.kuanghao11.cn

[R75] 导出环境变量
来源：http://dci.yj20258.top

export PATH="$HOME/bin:$PATH"
来源：http://old.ivvv.top

[R76] 使用临时文件
来源：http://spz.ydzc1.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://avu.yuanzhike.top

[R77] 读取用户输入
来源：http://enh.fanxiaobao.xyz

read -rp "请输入: " ans
来源：http://rdt.iojbl.cn

[R78] 交互式菜单
来源：http://dpx.svipenyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://szz.jinyuanbaomall.cn

[R79] 解析命令行选项
来源：http://bgw.zhixingplan.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mtf.shangyingyoupin.top

[R80] 查看脚本执行耗时
来源：http://lvm.yanxiufei.cn

time ./run.sh
来源：http://utj.iojbl.cn

================================================================================
来源：http://igp.birdmap.top

S. C / C++ 专题
来源：http://agd.zhijiandao.cn

================================================================================
来源：http://prt.nanxuanxn.top

[S01] C：Hello World
来源：http://zxl.vqdsnc.cn

#include <stdio.h>
来源：http://tox.xziqi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jrq.sxryk.cn

[S02] C：变量与格式化输出
来源：http://mgf.jqgfzy.top

int a = 10; printf("%d\n", a);
来源：http://zeg.hammf.cn

[S03] C：读入整数
来源：http://hqt.epnwcf.com

int x; scanf("%d", &x);
来源：http://xsz.gzhubu.top

[S04] C：字符串复制
来源：http://fhl.ivvv.top

char dst[32]; strcpy(dst, "hi");
来源：http://fbo.52xcode.cn

[S05] C：字符串长度
来源：http://egh.sufxvd.cn

strlen(s)
来源：http://ejr.uphjek.com

[S06] C：字符串比较
来源：http://yuj.quarkkingdee.top

strcmp(a, b) == 0
来源：http://vez.fanxiaobao.xyz

[S07] C：数组遍历求和
来源：http://dqq.sxryk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rnm.shangyingyoupin.top

[S08] C：动态内存分配与释放
来源：http://sxh.ctjpmb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dks.birdmap.top

[S09] C：结构体定义与初始化
来源：http://cee.tarul.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://upg.zhoulong.xyz

[S10] C：指针与解引用
来源：http://chu.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://bjo.jlsjyb.cn

[S11] C：逐行读文件
来源：http://txj.zhiwuduotai.top

FILE *f = fopen("a.txt", "r");
来源：http://aoc.guowangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dno.xinyue.icu

fclose(f);
来源：http://vyd.redwolf501.top

[S12] C：写文件
来源：http://vva.zhixingplan.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tju.chenzaomai.com

[S13] C：宏定义
来源：http://opt.snrcjt.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://agd.jqgfzy.top

[S14] C：枚举
来源：http://fek.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://ddf.yueranfly.top

[S15] C：类型转换
来源：http://fnr.sxryk.cn

(double) a / b
来源：http://xqv.epnwcf.com

[S16] C：位操作置位
来源：http://dcn.jqgfzy.top

x |= (1 << 3);
来源：http://ofs.jiagoushi.top

[S17] C：安全拼接字符串
来源：http://wze.iojbl.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ose.kuanghao11.cn

[S18] C：命令行参数
来源：http://dni.zdbjq.cn

int main(int argc, char **argv)
来源：http://bbf.jianghu66.top

[S19] C：快速排序
来源：http://uak.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mvd.hfpthk.cn

[S20] C：二分查找
来源：http://hgj.fehbvm.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sdx.c1oappe.top

[S21] C：字符类别判断
来源：http://scv.fanxiaobao.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aho.chenzaomai.com

[S22] C：字符串转数字
来源：http://umw.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wql.epnwcf.com

[S23] C：随机数
来源：http://iiv.yj202588.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wen.nanxuanxn.top

[S24] C：获取本地时间
来源：http://uxn.hnxiangtu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xwb.jyoumei.cn

[S25] C：内存拷贝
来源：http://lyg.zdbjq.cn

memcpy(dst, src, n);
来源：http://psr.chenzaomai.com

[S26] C：内存清零
来源：http://tan.yuanzhike.top


<!-- 参考信息 -->