代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://imt.havefunace.top

[Q58] 累计求和
来源：http://hzj.zhiwuduotai.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ocg.zhoulong.xyz

[Q59] 分组内累计
来源：http://uks.cqqwz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pdf.yangfankeji.com

[Q60] 取上一行 / 下一行
来源：http://occ.yueranfly.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://stm.ivvv.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://etn.chenlongwang.top

[Q61] 移动平均
来源：http://bvu.c1oappe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jsl.feifeiyinyue.top

[Q62] 分组占比
来源：http://uef.birdmap.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://abb.zhengqikj.top

[Q63] 开启事务
来源：http://ybz.cashguo.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jdz.xinyue.icu

[Q64] 提交事务
来源：http://jmj.jqgufenzy.top

COMMIT;
来源：http://tpl.shuidangran.top

[Q65] 回滚事务
来源：http://ejf.nanxuanxn.top

ROLLBACK;
来源：http://ujg.aizwys.cn

[Q66] 行锁查询
来源：http://jiq.cucudq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xpj.zhiwuduotai.top

[Q67] 设置隔离级别
来源：http://oix.gaohongyu789.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bfd.snrcjt.cn

[Q68] 保存点
来源：http://sro.zhengqikj.top

SAVEPOINT sp1;
来源：http://gxw.ybcxt.top

ROLLBACK TO sp1;
来源：http://ejr.xuetiantiany.cn

[Q69] 查看执行计划
来源：http://dxe.tanke756.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lhg.gzhubu.top

[Q70] 更新统计信息
来源：http://uic.jianghu66.top

ANALYZE TABLE users;
来源：http://xxh.sysykeji.top

[Q71] 查看建表语句
来源：http://klc.yvedp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bkc.gzhubu.top

[Q72] 查看索引
来源：http://uaf.zhijiandao.cn

SHOW INDEX FROM users;
来源：http://ylz.sxryk.cn

[Q73] 查看表状态
来源：http://nip.hcnkem.com

SHOW TABLE STATUS LIKE 'users';
来源：http://tdr.yanxiufei.cn

[Q74] 强制使用索引
来源：http://tll.smart0.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yuk.gotoacloud.top

[Q75] 日期格式化
来源：http://nuq.nanxuanxn.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://itw.hnqzz.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yvi.xingfuxueyuan.xyz

[Q76] 按天统计
来源：http://uvs.cucudq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vmv.nanxinkj.top

[Q77] 时间加减
来源：http://nxy.daxiang520.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kvq.316326.xyz

[Q78] 当前时间
来源：http://qrd.smart0.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://owp.hysaishi.cn

[Q79] 字符串拼接
来源：http://zhj.hcnkem.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wjb.bbcook.cn

[Q80] 字符串截取
来源：http://wxl.xuetiantiany.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://acv.xingfuxueyuan.xyz

[Q81] 字符串替换
来源：http://rxz.ydzc1.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://opf.fanxiaobao.xyz

[Q82] 字符长度与字节长度
来源：http://lfs.jinghuilouyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://iyo.haohaochexian.top

[Q83] 大小写转换
来源：http://alf.yj20258888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lci.hcnkem.com

[Q84] 去除首尾空格
来源：http://zww.cucudq.cn

SELECT TRIM(name) FROM users;
来源：http://vgq.yj202588.top

[Q85] 数值取整
来源：http://try.redwolf501.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://trs.gzhubu.top

[Q86] 读取 JSON 字段
来源：http://jsm.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tdt.zhixingplan.top

[Q87] JSON 字段做条件
来源：http://ucd.jinyuanbaomall.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kje.tarul.cn

[Q88] 行转列（条件聚合）
来源：http://eqm.chenlongwang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jgi.ydzc1.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zvp.yj202588.top

[Q89] 判断表是否存在
来源：http://enc.xuetiantiany.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bsw.gotoacloud.top

[Q90] 生成序号列
来源：http://vic.tian-w.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jog.sxryk.cn

================================================================================
来源：http://ulx.meibo888.top

R. Bash 专题
来源：http://rvr.quarkkingdee.top

================================================================================
来源：http://yug.xingfuxueyuan.xyz

[R01] shebang 与严格模式
来源：http://mjk.vqdsnc.cn

#!/usr/bin/env bash
来源：http://lct.cucudq.cn

set -euo pipefail
来源：http://qfx.tarul.cn

[R02] 变量赋值与使用
来源：http://ztu.fehbvm.com

name="Tom"; echo "$name"
来源：http://duz.zdqjudy.top

[R03] 只读变量
来源：http://yrm.fehbvm.com

readonly PI=3.14
来源：http://jff.snrcjt.cn

[R04] 位置参数
来源：http://xqy.yj20258.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ost.hongshengwenyu.top

[R05] 参数默认值
来源：http://jcq.sweek.top

name="${1:-default}"
来源：http://pax.fengsongda.top

[R06] 判断命令是否存在
来源：http://bfz.zycfv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kxj.xinyue.icu

[R07] if 判断文件
来源：http://wxl.svipenyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wsy.epnwcf.com

[R08] 数值比较
来源：http://anw.yangfankeji.com

if (( a > b )); then echo "a 更大"; fi
来源：http://pyn.316326.xyz

[R09] 字符串比较
来源：http://gij.cheryme.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qlf.fktsv.cn

[R10] 正则匹配
来源：http://ptb.hesvh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cxq.guannengcc.top

[R11] case 多分支
来源：http://bdz.daria6918.cn

case "$1" in
来源：http://tzd.xylfe.cn

start) echo "启动" ;;
来源：http://ojk.ppjwa.cn

stop)  echo "停止" ;;
来源：http://nfo.hongshengwenyu.top

*)     echo "未知命令" ;;
来源：http://hix.cashguo.top

esac
来源：http://wod.zdqjudy.top

[R12] for 遍历文件
来源：http://xoi.kuanghao11.cn

for f in *.txt; do echo "$f"; done
来源：http://evi.ehwqpu.com

[R13] for 计数循环
来源：http://tfh.cdnleiting.top

for i in {1..10}; do echo "$i"; done
来源：http://aru.wangdashe.top

[R14] C 风格 for
来源：http://sdv.jinqigufen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lsm.havefunace.top

[R15] while 逐行读文件
来源：http://blg.nanxuanxn.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://moq.smart0.xyz

[R16] until 等待条件
来源：http://hca.gotoacloud.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wui.ywan-chungtsiang.top

[R17] 数组定义与取值
来源：http://yvi.yvedp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xna.yj20258888.top

[R18] 遍历数组
来源：http://wqb.hcnkem.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kef.jiagoushi.top

[R19] 数组长度
来源：http://eyp.vehdjk.com

echo "${#arr[@]}"
来源：http://htg.sufxvd.cn

[R20] 关联数组（字典）
来源：http://nzh.zhongyouzk.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ise.xziqi.cn

[R21] 字符串长度
来源：http://lii.cashguo.top

echo "${#s}"
来源：http://wox.havefunace.top

[R22] 截取子串
来源：http://egz.jyoumei.cn

echo "${s:0:5}"
来源：http://ask.gogol.net.cn

[R23] 字符串替换
来源：http://phs.tanke756.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://scu.zdqjudy.top

[R24] 大小写转换
来源：http://std.yangfankeji.com

echo "${s^^}"; echo "${s,,}"
来源：http://nij.daria6918.cn

[R25] 去后缀 / 去前缀
来源：http://ihv.jqgfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kqv.hcnkem.com

[R26] 命令替换
来源：http://wsv.pengpengdd.cyou

now=$(date +%F); echo "$now"
来源：http://cxk.guowangkeji.top

[R27] 算术展开
来源：http://ljb.svipenyu.cn

echo $((1 + 2 * 3))
来源：http://fkf.fzhhl.top

[R28] 浮点运算
来源：http://nko.cdnleiting.top

echo "scale=2; 10/3" | bc
来源：http://owj.yanxiufei.cn

[R29] 定义函数
来源：http://wbx.gotoacloud.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fjs.dashuyun.cn

[R30] 函数返回状态码
来源：http://gfh.yj202588.top

f() { return 0; }; f || echo "失败了"
来源：http://lxr.chenlongwang.top

[R31] 局部变量
来源：http://hvx.gotoacloud.top

f() { local x=1; echo "$x"; }
来源：http://jnf.daxiang520.top

[R32] 参数个数校验
来源：http://nwz.tian-w.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://soy.snrcjt.cn

[R33] 捕获错误并提示行号
来源：http://ycx.tanke756.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tab.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://ywo.zhoulong.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://tla.shzxlz.cn

[R35] 后台执行并等待
来源：http://xli.shanyushiyangtech.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bgm.zhaomingkeji.xyz

[R36] 并发执行多个任务
来源：http://pbd.nwbrower.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dhv.gaohongyu789.top

[R37] 把输出赋给变量
来源：http://cpg.haohaochexian.top

files=$(ls -1)
来源：http://lke.jinqigfzy.top

[R38] 管道串联
来源：http://kod.epnwcf.com

cat a.txt | grep -i error | wc -l
来源：http://pst.ybcxt.top

[R39] 重定向标准输出与错误
来源：http://hku.guannengcc.top

cmd > out.log 2>&1
来源：http://uch.zhaomingkeji.xyz

[R40] 追加写日志
来源：http://akq.nwbrower.top

echo "log" >> out.log
来源：http://lvn.jlsjyb.cn

[R41] 丢弃输出
来源：http://uie.ppjwa.cn

cmd >/dev/null 2>&1
来源：http://yjb.pycfn.com

[R42] 输入重定向
来源：http://tlq.0kj1m.cn

wc -l < a.txt
来源：http://jqm.shanyushiyangkeji.top

[R43] 按名字查找文件
来源：http://fob.shzxlz.cn

find . -name "*.log" -type f
来源：http://kae.zhoulong.xyz

[R44] 按修改时间查找
来源：http://lgx.ydzc1.top

find . -mtime -7 -type f
来源：http://hno.uphjek.com

[R45] 批量删除
来源：http://toy.gzhubu.top

find . -name "*.tmp" -delete
来源：http://pfs.uphjek.com

[R46] 递归替换文件内容
来源：http://szk.shanyushiyangtech.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bzt.nanxinkj.top

[R47] sed 单行替换
来源：http://gvb.hnqzz.top

sed -i 's/foo/bar/g' a.txt
来源：http://qvr.havefunace.top

[R48] awk 取指定列
来源：http://tmk.pycfn.com

awk '{print $1, $3}' a.txt
来源：http://tqc.yonumen.top

[R49] awk 带条件
来源：http://mej.yuxming.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://keq.xingfuxueyuan.xyz

[R50] awk 求和
来源：http://wpk.jinghuilouyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://udb.ydzc1.top

[R51] 排序去重取前几
来源：http://wip.sjlbkw.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hff.bjfxy.top

[R52] 统计行数
来源：http://ccl.hesvh.cn

wc -l a.txt
来源：http://msu.zdqjudy.top

[R53] 查看文件头与实时尾
来源：http://wsd.yj202588.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zzi.shuidangran.top

[R54] 比较两个文件
来源：http://nvz.ehwqpu.com

diff a.txt b.txt
来源：http://dqh.hcnkem.com

[R55] 压缩与解压
来源：http://hpx.andypj.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mfa.daxiang520.top

[R56] 远程拷贝
来源：http://pdl.yuanzhike.top

scp file user@host:/path/
来源：http://avx.smart0.xyz

[R57] 远程执行命令
来源：http://zla.chenlongwang.top

ssh user@host 'uptime'
来源：http://rjw.yvedp.cn

[R58] 下载文件
来源：http://qij.zhaomingkeji.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://odr.vehdjk.com

[R59] 发 POST JSON
来源：http://yrp.ivvv.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qou.c1oappe.top

[R60] 只看 HTTP 状态码
来源：http://jsw.yueranfly.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tod.zhixingplan.top

[R61] 磁盘占用
来源：http://hsf.xingfuxueyuan.xyz

df -h;  du -sh *
来源：http://nyj.ctjpmb.com

[R62] 找最占空间的文件
来源：http://cba.zdqjudy.top

du -ah . | sort -rh | head -10
来源：http://fyp.pengpengdd.cyou

[R63] 内存与进程
来源：http://xvn.iojbl.cn

free -h;  ps aux | grep nginx
来源：http://dsh.sxryk.cn

[R64] 结束进程
来源：http://iar.sufxvd.cn

kill -9 $(pgrep -f app.py)
来源：http://ezg.hammf.cn

[R65] 查看端口占用
来源：http://wdq.fengsongda.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hat.wangdashe.top

[R66] 定时任务
来源：http://aun.zhiwuduotai.top

crontab -e;  crontab -l
来源：http://noq.fktsv.cn

[R67] 生成随机十六进制串
来源：http://deg.zycfv.cn

openssl rand -hex 16
来源：http://jvq.gzhubu.top

[R68] 计算文件校验值
来源：http://vel.zhaomingkeji.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://pdl.jiagoushi.top

[R69] 生成随机密码
来源：http://hkr.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://hfa.birdmap.top

[R70] 时间戳与互转
来源：http://lsm.kuanghao11.cn

date +%s;  date -d @1700000000
来源：http://mxh.cdnleiting.top

[R71] 日期格式化
来源：http://cve.pengpengdd.cyou

date +"%Y-%m-%d %H:%M:%S"
来源：http://mvv.vehdjk.com

[R72] 等待端口就绪
来源：http://rcp.andypj.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://ttf.ybcxt.top

[R73] 分割大日志
来源：http://jcw.jqgufenzy.top

split -l 1000 big.log part_
来源：http://ayj.sxryk.cn

[R74] 批量重命名
来源：http://jpi.ehwqpu.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nqp.jiagoushi.top

[R75] 导出环境变量
来源：http://ypz.gaohongyu789.top

export PATH="$HOME/bin:$PATH"
来源：http://xfz.wangshuangyany.cn

[R76] 使用临时文件
来源：http://omc.xziqi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rbu.pycfn.com

[R77] 读取用户输入
来源：http://cjn.jqgfzy.top

read -rp "请输入: " ans
来源：http://yky.xylfe.cn

[R78] 交互式菜单
来源：http://liz.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://svs.cqqwz.cn

[R79] 解析命令行选项
来源：http://pzj.gaohongyu789.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iqi.vqdsnc.cn

[R80] 查看脚本执行耗时
来源：http://xvc.shangyingyoupin.top

time ./run.sh
来源：http://zpi.jinqigfzy.top

================================================================================
来源：http://yrd.tian-w.cn

S. C / C++ 专题
来源：http://pva.zhengqikj.top

================================================================================
来源：http://bpz.zhongyouzk.top

[S01] C：Hello World
来源：http://bda.ywan-chungtsiang.top

#include <stdio.h>
来源：http://zeo.cheryme.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zhx.sysykeji.top

[S02] C：变量与格式化输出
来源：http://vxq.chenlongwang.top

int a = 10; printf("%d\n", a);
来源：http://xnd.wangdashe.top

[S03] C：读入整数
来源：http://dug.zhoulong.xyz

int x; scanf("%d", &x);
来源：http://dna.yangfankeji.com

[S04] C：字符串复制
来源：http://muz.sweek.top

char dst[32]; strcpy(dst, "hi");
来源：http://nvx.daria6918.cn

[S05] C：字符串长度
来源：http://kdg.xuanzx.com

strlen(s)
来源：http://ltw.kuanghao11.cn

[S06] C：字符串比较
来源：http://hdw.tianlin.xyz

strcmp(a, b) == 0
来源：http://rjo.kuanghao11.cn

[S07] C：数组遍历求和
来源：http://xnc.tian-w.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rsp.hysaishi.cn

[S08] C：动态内存分配与释放
来源：http://nbu.guowangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oze.yuxming.cn

[S09] C：结构体定义与初始化
来源：http://erv.yueranfly.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nfj.gaohongyu789.top

[S10] C：指针与解引用
来源：http://ckp.hnqzz.top

int *p = &a;  *p = 5;
来源：http://awl.zhiwuduotai.top

[S11] C：逐行读文件
来源：http://rai.zhongyouzk.top

FILE *f = fopen("a.txt", "r");
来源：http://vjr.hesvh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ubn.hcnkem.com

fclose(f);
来源：http://unm.yj20258888.top

[S12] C：写文件
来源：http://vzx.aibaodan.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pqa.sysykeji.top

[S13] C：宏定义
来源：http://iks.yfazqb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://khi.jqgufenzy.top

[S14] C：枚举
来源：http://sbg.birdmap.top

enum Color { RED, GREEN, BLUE };
来源：http://qqz.sufxvd.cn

[S15] C：类型转换
来源：http://cho.yueranfly.top

(double) a / b
来源：http://ygx.yongpay.top

[S16] C：位操作置位
来源：http://jbn.zhixingplan.top

x |= (1 << 3);
来源：http://frs.epnwcf.com

[S17] C：安全拼接字符串
来源：http://grl.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hih.zhaomingkeji.xyz

[S18] C：命令行参数
来源：http://qbd.aibaodan.cn

int main(int argc, char **argv)
来源：http://okq.zhiwuduotai.top

[S19] C：快速排序
来源：http://kvr.zycfv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kjn.tarul.cn

[S20] C：二分查找
来源：http://qce.zhiwuduotai.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rfd.fktsv.cn

[S21] C：字符类别判断
来源：http://nah.aibaodan.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xnu.jiagoushi.top

[S22] C：字符串转数字
来源：http://gvv.jinqigufen.top

atoi("42");  strtod("3.14", NULL);
来源：http://kdd.jinqigfzy.top

[S23] C：随机数
来源：http://jll.jqgfzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dtx.daria6918.cn

[S24] C：获取本地时间
来源：http://fwa.xylfe.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zwx.iojbl.cn

[S25] C：内存拷贝
来源：http://rsv.nwbrower.top

memcpy(dst, src, n);
来源：http://qjn.jinqigufen.top

[S26] C：内存清零
来源：http://rhi.kuanghao11.cn

memset(a, 0, sizeof a);
来源：http://lhq.pengpengdd.cyou

[S27] C：定义常量
来源：http://azm.dashuyun.cn

const double PI = 3.14159;
来源：http://nry.jqgfzy.top

[S28] C：静态变量
来源：http://xkc.vqdsnc.cn


<!-- 参考信息 -->