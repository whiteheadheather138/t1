代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bpj.yongpay.top

[Q56] 密集排名（并列不占位）
来源：http://xtq.cdnleiting.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jwf.chenzaomai.com

[Q57] 行号
来源：http://llk.zhaomingkeji.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://krx.sysykeji.top

[Q58] 累计求和
来源：http://mme.ivvv.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gvs.zhoulong.xyz

[Q59] 分组内累计
来源：http://nmk.sysykeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://duz.andypj.xyz

[Q60] 取上一行 / 下一行
来源：http://bve.iojbl.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uic.52xcode.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lek.snrcjt.cn

[Q61] 移动平均
来源：http://znx.havefunace.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oyd.chenzaomai.com

[Q62] 分组占比
来源：http://wbr.shuidangran.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bly.yuxming.cn

[Q63] 开启事务
来源：http://knd.bjfxy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://goh.zhoulong.xyz

[Q64] 提交事务
来源：http://cuc.hywenlv.cn

COMMIT;
来源：http://ocq.c1oappe.top

[Q65] 回滚事务
来源：http://cdj.zhaomingkeji.xyz

ROLLBACK;
来源：http://vhp.yfazqb.com

[Q66] 行锁查询
来源：http://rfc.yvedp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://occ.dashuyun.cn

[Q67] 设置隔离级别
来源：http://puz.jianghu66.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://are.hammf.cn

[Q68] 保存点
来源：http://xqk.fzhhl.top

SAVEPOINT sp1;
来源：http://nql.yfazqb.com

ROLLBACK TO sp1;
来源：http://iks.zhoulong.xyz

[Q69] 查看执行计划
来源：http://muu.jqgufenzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fad.sxryk.cn

[Q70] 更新统计信息
来源：http://ehd.wangshuangyany.cn

ANALYZE TABLE users;
来源：http://hlf.vehdjk.com

[Q71] 查看建表语句
来源：http://rzh.hysaishi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ays.yanxiufei.cn

[Q72] 查看索引
来源：http://bms.xuanzx.com

SHOW INDEX FROM users;
来源：http://zpq.yvedp.cn

[Q73] 查看表状态
来源：http://gdq.gaohongyu789.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lyv.zycfv.cn

[Q74] 强制使用索引
来源：http://ewr.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hbd.jlsjyb.cn

[Q75] 日期格式化
来源：http://zwn.fktsv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://biz.pengpengdd.cyou

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bmd.gzhubu.top

[Q76] 按天统计
来源：http://ako.gotoacloud.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://snk.jlsjyb.cn

[Q77] 时间加减
来源：http://deh.sweek.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ahn.yuanzhike.top

[Q78] 当前时间
来源：http://yrx.yvedp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://txn.316326.xyz

[Q79] 字符串拼接
来源：http://ecn.sjlbkw.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pgn.zdbjq.cn

[Q80] 字符串截取
来源：http://xjw.fanxiaobao.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rpc.shuidangran.top

[Q81] 字符串替换
来源：http://kzu.nwbrower.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://juc.jqgufenzy.top

[Q82] 字符长度与字节长度
来源：http://ubu.zhongyouzk.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ubl.epnwcf.com

[Q83] 大小写转换
来源：http://gdp.havefunace.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uuo.hongshengwenyu.top

[Q84] 去除首尾空格
来源：http://xvb.chenjidiqi.icu

SELECT TRIM(name) FROM users;
来源：http://dht.vehdjk.com

[Q85] 数值取整
来源：http://gwh.yj20258888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jmg.cucudq.cn

[Q86] 读取 JSON 字段
来源：http://pxy.xuanzx.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yzv.0kj1m.cn

[Q87] JSON 字段做条件
来源：http://bdx.jinyuanbaomall.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bml.tianlin.xyz

[Q88] 行转列（条件聚合）
来源：http://wxg.hesvh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pai.jlsjyb.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kkg.xuanzx.com

[Q89] 判断表是否存在
来源：http://luw.smart0.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://frw.yuxming.cn

[Q90] 生成序号列
来源：http://epy.fzhhl.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qqw.yangfankeji.com

================================================================================
来源：http://wte.xingfuxueyuan.xyz

R. Bash 专题
来源：http://tkf.yueranfly.top

================================================================================
来源：http://lyf.bbcook.cn

[R01] shebang 与严格模式
来源：http://csj.haohaochexian.top

#!/usr/bin/env bash
来源：http://ksf.xuetiantiany.cn

set -euo pipefail
来源：http://vxu.daria6918.cn

[R02] 变量赋值与使用
来源：http://bin.svipenyu.cn

name="Tom"; echo "$name"
来源：http://tex.fktsv.cn

[R03] 只读变量
来源：http://nnq.hesvh.cn

readonly PI=3.14
来源：http://ntx.jqgufenzy.top

[R04] 位置参数
来源：http://kry.sjlbkw.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dkh.sufxvd.cn

[R05] 参数默认值
来源：http://qkj.ydjk.org.cn

name="${1:-default}"
来源：http://ruo.ehwqpu.com

[R06] 判断命令是否存在
来源：http://txx.snrcjt.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tdp.gotoacloud.top

[R07] if 判断文件
来源：http://gun.ivvv.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ely.svipenyu.cn

[R08] 数值比较
来源：http://sws.pycfn.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ent.ehwqpu.com

[R09] 字符串比较
来源：http://rvf.fengsongda.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fcv.smart0.xyz

[R10] 正则匹配
来源：http://bre.zdqjudy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jht.tian-w.cn

[R11] case 多分支
来源：http://jou.xinyue.icu

case "$1" in
来源：http://slm.ivvv.top

start) echo "启动" ;;
来源：http://xuj.c1oappe.top

stop)  echo "停止" ;;
来源：http://vkb.jinghuilouyu.cn

*)     echo "未知命令" ;;
来源：http://tkx.zycfv.cn

esac
来源：http://lzm.yuanzhike.top

[R12] for 遍历文件
来源：http://qkr.hammf.cn

for f in *.txt; do echo "$f"; done
来源：http://afo.uphjek.com

[R13] for 计数循环
来源：http://zkf.hnxiangtu.top

for i in {1..10}; do echo "$i"; done
来源：http://vrz.yangfankeji.com

[R14] C 风格 for
来源：http://yas.xingfuxueyuan.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rfb.sxryk.cn

[R15] while 逐行读文件
来源：http://iqc.snrcjt.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cxn.nanxuanxn.top

[R16] until 等待条件
来源：http://rog.zhaomingkeji.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gua.snrcjt.cn

[R17] 数组定义与取值
来源：http://cuo.zdbjq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rdi.yanxiufei.cn

[R18] 遍历数组
来源：http://xnz.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eun.fzhhl.top

[R19] 数组长度
来源：http://utr.sxryk.cn

echo "${#arr[@]}"
来源：http://ejf.vehdjk.com

[R20] 关联数组（字典）
来源：http://eme.chenzaomai.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zbl.kuanghao11.cn

[R21] 字符串长度
来源：http://ges.tanke756.top

echo "${#s}"
来源：http://suq.ydzc1.top

[R22] 截取子串
来源：http://xsi.shzxlz.cn

echo "${s:0:5}"
来源：http://zrs.xylfe.cn

[R23] 字符串替换
来源：http://kms.chenzaomai.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pdk.kuanghao11.cn

[R24] 大小写转换
来源：http://wex.zycfv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ueh.cqqwz.cn

[R25] 去后缀 / 去前缀
来源：http://pdm.xuanzx.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://tfl.hcnkem.com

[R26] 命令替换
来源：http://byt.ywan-chungtsiang.top

now=$(date +%F); echo "$now"
来源：http://atz.cashguo.top

[R27] 算术展开
来源：http://rhk.cheryme.top

echo $((1 + 2 * 3))
来源：http://cse.hammf.cn

[R28] 浮点运算
来源：http://vpq.wangdashe.top

echo "scale=2; 10/3" | bc
来源：http://byr.snrcjt.cn

[R29] 定义函数
来源：http://xne.jyoumei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://imr.316326.xyz

[R30] 函数返回状态码
来源：http://gou.shanyushiyangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://mpj.ctjpmb.com

[R31] 局部变量
来源：http://czd.yj202588.top

f() { local x=1; echo "$x"; }
来源：http://bcd.jinghuilouyu.cn

[R32] 参数个数校验
来源：http://ivm.xziqi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qww.hongshengwenyu.top

[R33] 捕获错误并提示行号
来源：http://cfq.jlsjyb.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hbz.jinqigfzy.top

[R34] 退出时清理
来源：http://cqh.xuetiantiany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qpy.shanyushiyangtech.top

[R35] 后台执行并等待
来源：http://xxg.smart0.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://cmw.c1oappe.top

[R36] 并发执行多个任务
来源：http://xww.nanxuanxn.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tsf.zhixingplan.top

[R37] 把输出赋给变量
来源：http://bpo.jinqigfzy.top

files=$(ls -1)
来源：http://ial.daxiang520.top

[R38] 管道串联
来源：http://wli.zdbjq.cn

cat a.txt | grep -i error | wc -l
来源：http://lgo.yfazqb.com

[R39] 重定向标准输出与错误
来源：http://qbo.zhongyouzk.top

cmd > out.log 2>&1
来源：http://tzz.jiagoushi.top

[R40] 追加写日志
来源：http://ojb.snrcjt.cn

echo "log" >> out.log
来源：http://spw.c1oappe.top

[R41] 丢弃输出
来源：http://ifk.hysaishi.cn

cmd >/dev/null 2>&1
来源：http://nwg.chenlongwang.top

[R42] 输入重定向
来源：http://cch.chenzaomai.com

wc -l < a.txt
来源：http://iuy.ehwqpu.com

[R43] 按名字查找文件
来源：http://yzo.gotoacloud.top

find . -name "*.log" -type f
来源：http://tlf.ivvv.top

[R44] 按修改时间查找
来源：http://ovq.xuetiantiany.cn

find . -mtime -7 -type f
来源：http://cvv.redwolf501.top

[R45] 批量删除
来源：http://bfn.jyoumei.cn

find . -name "*.tmp" -delete
来源：http://rvn.daria6918.cn

[R46] 递归替换文件内容
来源：http://hvi.jyoumei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qmt.ehwqpu.com

[R47] sed 单行替换
来源：http://lst.chenjidiqi.icu

sed -i 's/foo/bar/g' a.txt
来源：http://uur.hnxiangtu.top

[R48] awk 取指定列
来源：http://eim.xylfe.cn

awk '{print $1, $3}' a.txt
来源：http://yam.uphjek.com

[R49] awk 带条件
来源：http://ewj.ivvv.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ngz.sxryk.cn

[R50] awk 求和
来源：http://rdb.aizwys.cn

awk '{s += $2} END {print s}' a.txt
来源：http://naf.52xcode.cn

[R51] 排序去重取前几
来源：http://lop.shzxlz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vfm.shuidangran.top

[R52] 统计行数
来源：http://ksa.jianghu66.top

wc -l a.txt
来源：http://cus.birdmap.top

[R53] 查看文件头与实时尾
来源：http://cql.tanke756.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://unq.smart0.xyz

[R54] 比较两个文件
来源：http://xas.feifeiyinyue.top

diff a.txt b.txt
来源：http://qdo.nanxuanxn.top

[R55] 压缩与解压
来源：http://nyq.haohaochexian.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mgl.yj20258888.top

[R56] 远程拷贝
来源：http://axm.jlsjyb.cn

scp file user@host:/path/
来源：http://fsu.kuanghao11.cn

[R57] 远程执行命令
来源：http://ifp.meibo888.top

ssh user@host 'uptime'
来源：http://irp.cdnleiting.top

[R58] 下载文件
来源：http://xxh.316326.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jfz.guannengcc.top

[R59] 发 POST JSON
来源：http://ofi.meibo888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iqw.ctjpmb.com

[R60] 只看 HTTP 状态码
来源：http://qnf.birdmap.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://led.yj20258.top

[R61] 磁盘占用
来源：http://hdk.tian-w.cn

df -h;  du -sh *
来源：http://xud.yuxming.cn

[R62] 找最占空间的文件
来源：http://vrh.chenjidiqi.icu

du -ah . | sort -rh | head -10
来源：http://dim.cqqwz.cn

[R63] 内存与进程
来源：http://sqb.jinqigfzy.top

free -h;  ps aux | grep nginx
来源：http://pkp.zhongyouzk.top

[R64] 结束进程
来源：http://xca.fktsv.cn

kill -9 $(pgrep -f app.py)
来源：http://tre.hnxiangtu.top

[R65] 查看端口占用
来源：http://hfe.jiagoushi.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mlj.birdmap.top

[R66] 定时任务
来源：http://dfh.gotoacloud.top

crontab -e;  crontab -l
来源：http://lqf.feifeiyinyue.top

[R67] 生成随机十六进制串
来源：http://mma.gzhubu.top

openssl rand -hex 16
来源：http://hij.jinqigufen.top

[R68] 计算文件校验值
来源：http://rnv.bbcook.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wxi.shzxlz.cn

[R69] 生成随机密码
来源：http://vli.c1oappe.top

head -c 16 /dev/urandom | base64
来源：http://kja.yvedp.cn

[R70] 时间戳与互转
来源：http://qwt.yuxming.cn

date +%s;  date -d @1700000000
来源：http://kqa.guannengcc.top

[R71] 日期格式化
来源：http://aha.ivvv.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pwg.gogol.net.cn

[R72] 等待端口就绪
来源：http://bmf.ivvv.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ezv.tianlin.xyz

[R73] 分割大日志
来源：http://osk.yj20258.top

split -l 1000 big.log part_
来源：http://hhb.tanke756.top

[R74] 批量重命名
来源：http://jxw.hammf.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zkg.sjlbkw.cn

[R75] 导出环境变量
来源：http://tqc.feifeiyinyue.top

export PATH="$HOME/bin:$PATH"
来源：http://fgq.yj20258888.top

[R76] 使用临时文件
来源：http://lso.jinqigfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gth.tanke756.top

[R77] 读取用户输入
来源：http://jay.zhiwuduotai.top

read -rp "请输入: " ans
来源：http://xla.jinyuanbaomall.cn

[R78] 交互式菜单
来源：http://mpv.dianchejie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mzp.zhoulong.xyz

[R79] 解析命令行选项
来源：http://ola.yfazqb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://csn.sjlbkw.cn

[R80] 查看脚本执行耗时
来源：http://ina.wangdashe.top

time ./run.sh
来源：http://uzf.pycfn.com

================================================================================
来源：http://qbh.aizwys.cn

S. C / C++ 专题
来源：http://boi.ywan-chungtsiang.top

================================================================================
来源：http://doe.zhoulong.xyz

[S01] C：Hello World
来源：http://hrp.nanxuanxn.top

#include <stdio.h>
来源：http://wqb.jqgufenzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://thz.ppjwa.cn

[S02] C：变量与格式化输出
来源：http://bsw.ehwqpu.com

int a = 10; printf("%d\n", a);
来源：http://fgo.tarul.cn

[S03] C：读入整数
来源：http://dlb.zhijiandao.cn

int x; scanf("%d", &x);
来源：http://jms.epnwcf.com

[S04] C：字符串复制
来源：http://bqg.jyoumei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vwt.andypj.xyz

[S05] C：字符串长度
来源：http://ich.9152youxi.cn

strlen(s)
来源：http://kud.zdbjq.cn

[S06] C：字符串比较
来源：http://dil.yangfankeji.com

strcmp(a, b) == 0
来源：http://bsa.c1oappe.top

[S07] C：数组遍历求和
来源：http://hjs.quarkkingdee.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nin.xingfuxueyuan.xyz

[S08] C：动态内存分配与释放
来源：http://ybj.nanxinkj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yio.ywan-chungtsiang.top

[S09] C：结构体定义与初始化
来源：http://rxq.gaohongyu789.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nne.ybcxt.top

[S10] C：指针与解引用
来源：http://rig.gotoacloud.top

int *p = &a;  *p = 5;
来源：http://huq.feifeiyinyue.top

[S11] C：逐行读文件
来源：http://brp.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://rny.shangyingyoupin.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rns.zdbjq.cn

fclose(f);
来源：http://ndc.9152youxi.cn

[S12] C：写文件
来源：http://ati.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://exj.chenlongwang.top

[S13] C：宏定义
来源：http://wnr.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://quy.andypj.xyz

[S14] C：枚举
来源：http://hsv.jinqigufen.top

enum Color { RED, GREEN, BLUE };
来源：http://wxc.xuetiantiany.cn

[S15] C：类型转换
来源：http://dac.hcnkem.com

(double) a / b
来源：http://xoe.quarkkingdee.top

[S16] C：位操作置位
来源：http://iab.zhiwuduotai.top

x |= (1 << 3);
来源：http://gmq.jlsjyb.cn

[S17] C：安全拼接字符串
来源：http://ito.hywenlv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hlr.ivvv.top

[S18] C：命令行参数
来源：http://ixt.gogol.net.cn

int main(int argc, char **argv)
来源：http://loo.chenlongwang.top

[S19] C：快速排序
来源：http://ugf.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://pun.zhiwuduotai.top

[S20] C：二分查找
来源：http://bdi.jiagoushi.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://olt.jinghuilouyu.cn

[S21] C：字符类别判断
来源：http://bcc.chenjidiqi.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tbk.fehbvm.com

[S22] C：字符串转数字
来源：http://too.yangfankeji.com

atoi("42");  strtod("3.14", NULL);
来源：http://wgg.zhongyouzk.top

[S23] C：随机数
来源：http://eho.tarul.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vte.iojbl.cn

[S24] C：获取本地时间
来源：http://xzn.guannengcc.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://plp.daria6918.cn

[S25] C：内存拷贝
来源：http://isi.sweek.top

memcpy(dst, src, n);
来源：http://zik.hnqzz.top

[S26] C：内存清零
来源：http://muv.gotoacloud.top


<!-- 参考信息 -->