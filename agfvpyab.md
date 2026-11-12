代发 wailian999

[Q65] 回滚事务
来源：http://vsv.hnxiangtu.top

ROLLBACK;
来源：http://izw.zhiwuduotai.top

[Q66] 行锁查询
来源：http://ppw.xylfe.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fep.yfazqb.com

[Q67] 设置隔离级别
来源：http://cuz.yonumen.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ety.tanke756.top

[Q68] 保存点
来源：http://dvc.jinyuanbaomall.cn

SAVEPOINT sp1;
来源：http://pwy.pengpengdd.cyou

ROLLBACK TO sp1;
来源：http://uyp.shanyushiyangkeji.top

[Q69] 查看执行计划
来源：http://wax.hammf.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lan.feifeiyinyue.top

[Q70] 更新统计信息
来源：http://xoj.mhx1999.top

ANALYZE TABLE users;
来源：http://rjq.sjlbkw.cn

[Q71] 查看建表语句
来源：http://zfc.smart0.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rhn.nanxinkj.top

[Q72] 查看索引
来源：http://tug.cucudq.cn

SHOW INDEX FROM users;
来源：http://kiq.hywenlv.cn

[Q73] 查看表状态
来源：http://bnl.wangshuangyany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://igm.wangshuangyany.cn

[Q74] 强制使用索引
来源：http://mfo.sysykeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bdk.zhijiandao.cn

[Q75] 日期格式化
来源：http://kft.hnqzz.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mpe.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wgx.birdmap.top

[Q76] 按天统计
来源：http://prb.snrcjt.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zua.nanxuanxn.top

[Q77] 时间加减
来源：http://hnp.zycfv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ggb.wangdashe.top

[Q78] 当前时间
来源：http://npt.hcnkem.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://end.xuetiantiany.cn

[Q79] 字符串拼接
来源：http://xxd.cheryme.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hvw.hesvh.cn

[Q80] 字符串截取
来源：http://mho.yfazqb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eca.zdbjq.cn

[Q81] 字符串替换
来源：http://rzz.bbcook.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lsd.cqqwz.cn

[Q82] 字符长度与字节长度
来源：http://smt.xingfuxueyuan.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wad.redwolf501.top

[Q83] 大小写转换
来源：http://ofk.hcnkem.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jrg.yanxiufei.cn

[Q84] 去除首尾空格
来源：http://snn.zhijiandao.cn

SELECT TRIM(name) FROM users;
来源：http://gwi.tian-w.cn

[Q85] 数值取整
来源：http://acf.xuetiantiany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jun.aibaodan.cn

[Q86] 读取 JSON 字段
来源：http://ija.xuanzx.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lmh.chenjidiqi.icu

[Q87] JSON 字段做条件
来源：http://jdn.9152youxi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eup.fehbvm.com

[Q88] 行转列（条件聚合）
来源：http://kqc.tanke756.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kqt.jianghu66.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rci.svipenyu.cn

[Q89] 判断表是否存在
来源：http://yab.yonumen.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ahr.ydzc1.top

[Q90] 生成序号列
来源：http://vnf.xylfe.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sok.wangdashe.top

================================================================================
来源：http://kcw.xziqi.cn

R. Bash 专题
来源：http://ucj.xinyue.icu

================================================================================
来源：http://nle.cheryme.top

[R01] shebang 与严格模式
来源：http://gxq.hysaishi.cn

#!/usr/bin/env bash
来源：http://rcg.fengsongda.top

set -euo pipefail
来源：http://uyw.yj20258888.top

[R02] 变量赋值与使用
来源：http://tvx.fengsongda.top

name="Tom"; echo "$name"
来源：http://rhs.zhijiandao.cn

[R03] 只读变量
来源：http://ram.zdqjudy.top

readonly PI=3.14
来源：http://wae.hesvh.cn

[R04] 位置参数
来源：http://cqx.jinghuilouyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mve.zhengqikj.top

[R05] 参数默认值
来源：http://ovp.shanyushiyangtech.top

name="${1:-default}"
来源：http://pct.gzhubu.top

[R06] 判断命令是否存在
来源：http://wpf.zhengqikj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bgo.cqqwz.cn

[R07] if 判断文件
来源：http://lbd.quarkkingdee.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tls.hammf.cn

[R08] 数值比较
来源：http://dla.ydzc1.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zxy.ywan-chungtsiang.top

[R09] 字符串比较
来源：http://tls.chenjidiqi.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jcf.dianchejie.cn

[R10] 正则匹配
来源：http://pvf.mhx1999.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ppb.kuanghao11.cn

[R11] case 多分支
来源：http://usu.hnqzz.top

case "$1" in
来源：http://cjy.tarul.cn

start) echo "启动" ;;
来源：http://tcg.nanxinkj.top

stop)  echo "停止" ;;
来源：http://nhk.wangshuangyany.cn

*)     echo "未知命令" ;;
来源：http://ycw.wangdashe.top

esac
来源：http://dcn.jinghuilouyu.cn

[R12] for 遍历文件
来源：http://hhq.fzhhl.top

for f in *.txt; do echo "$f"; done
来源：http://prc.cqqwz.cn

[R13] for 计数循环
来源：http://lkg.tianlin.xyz

for i in {1..10}; do echo "$i"; done
来源：http://gwk.zycfv.cn

[R14] C 风格 for
来源：http://oec.shzxlz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ort.hysaishi.cn

[R15] while 逐行读文件
来源：http://lez.c1oappe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vlh.hesvh.cn

[R16] until 等待条件
来源：http://uqk.vqdsnc.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gel.hysaishi.cn

[R17] 数组定义与取值
来源：http://gky.dashuyun.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mvb.jlsjyb.cn

[R18] 遍历数组
来源：http://tkx.nwbrower.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nbl.gaohongyu789.top

[R19] 数组长度
来源：http://cqg.hongshengwenyu.top

echo "${#arr[@]}"
来源：http://rdc.sweek.top

[R20] 关联数组（字典）
来源：http://jdo.ybcxt.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://efw.cdnleiting.top

[R21] 字符串长度
来源：http://npt.hongshengwenyu.top

echo "${#s}"
来源：http://ipc.yj202588.top

[R22] 截取子串
来源：http://pmt.sxryk.cn

echo "${s:0:5}"
来源：http://qmx.dianchejie.cn

[R23] 字符串替换
来源：http://ubv.gaohongyu789.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jow.sjlbkw.cn

[R24] 大小写转换
来源：http://bhb.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://kto.ydjk.org.cn

[R25] 去后缀 / 去前缀
来源：http://cpx.hammf.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dgq.xuetiantiany.cn

[R26] 命令替换
来源：http://zcu.feifeiyinyue.top

now=$(date +%F); echo "$now"
来源：http://clw.yonumen.top

[R27] 算术展开
来源：http://wvl.xingfuxueyuan.xyz

echo $((1 + 2 * 3))
来源：http://asn.pengpengdd.cyou

[R28] 浮点运算
来源：http://rhj.xuanzx.com

echo "scale=2; 10/3" | bc
来源：http://yfv.uphjek.com

[R29] 定义函数
来源：http://ytb.meibo888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dhg.52xcode.cn

[R30] 函数返回状态码
来源：http://ing.jqgfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://xuy.xuanzx.com

[R31] 局部变量
来源：http://cxp.cheryme.top

f() { local x=1; echo "$x"; }
来源：http://tbc.jinqigufen.top

[R32] 参数个数校验
来源：http://ftt.wangshuangyany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://snf.zhaomingkeji.xyz

[R33] 捕获错误并提示行号
来源：http://zwl.birdmap.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nmy.jinqigfzy.top

[R34] 退出时清理
来源：http://xkz.chenjidiqi.icu

trap 'rm -f "$tmp"' EXIT
来源：http://gfd.ydzc1.top

[R35] 后台执行并等待
来源：http://muy.guannengcc.top

sleep 5 & pid=$!; wait "$pid"
来源：http://oqq.guowangkeji.top

[R36] 并发执行多个任务
来源：http://cum.zhongyouzk.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kbz.jinqigufen.top

[R37] 把输出赋给变量
来源：http://wgc.hammf.cn

files=$(ls -1)
来源：http://mbt.zhiwuduotai.top

[R38] 管道串联
来源：http://zqc.cdnleiting.top

cat a.txt | grep -i error | wc -l
来源：http://szy.zhiwuduotai.top

[R39] 重定向标准输出与错误
来源：http://tio.snrcjt.cn

cmd > out.log 2>&1
来源：http://wrj.yanxiufei.cn

[R40] 追加写日志
来源：http://flf.guowangkeji.top

echo "log" >> out.log
来源：http://jjw.iojbl.cn

[R41] 丢弃输出
来源：http://zlx.cqqwz.cn

cmd >/dev/null 2>&1
来源：http://jws.quarkkingdee.top

[R42] 输入重定向
来源：http://vqh.fanxiaobao.xyz

wc -l < a.txt
来源：http://mhe.jiagoushi.top

[R43] 按名字查找文件
来源：http://ifk.yangfankeji.com

find . -name "*.log" -type f
来源：http://pim.hongshengwenyu.top

[R44] 按修改时间查找
来源：http://jxt.hammf.cn

find . -mtime -7 -type f
来源：http://ciu.zdqjudy.top

[R45] 批量删除
来源：http://txp.uphjek.com

find . -name "*.tmp" -delete
来源：http://zzx.yongpay.top

[R46] 递归替换文件内容
来源：http://xsj.hcnkem.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qym.0kj1m.cn

[R47] sed 单行替换
来源：http://lpk.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://fmr.zhongyouzk.top

[R48] awk 取指定列
来源：http://dut.hfpthk.cn

awk '{print $1, $3}' a.txt
来源：http://izs.yvedp.cn

[R49] awk 带条件
来源：http://pip.guannengcc.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ipy.gogol.net.cn

[R50] awk 求和
来源：http://pdv.ppjwa.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dpb.shangyingyoupin.top

[R51] 排序去重取前几
来源：http://paj.zycfv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qqd.uphjek.com

[R52] 统计行数
来源：http://xkd.dianchejie.cn

wc -l a.txt
来源：http://kqf.dianchejie.cn

[R53] 查看文件头与实时尾
来源：http://ssm.haohaochexian.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aid.fktsv.cn

[R54] 比较两个文件
来源：http://sei.fktsv.cn

diff a.txt b.txt
来源：http://yxk.shangyingyoupin.top

[R55] 压缩与解压
来源：http://dep.epnwcf.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mty.yfazqb.com

[R56] 远程拷贝
来源：http://ofj.gzhubu.top

scp file user@host:/path/
来源：http://rjh.ctjpmb.com

[R57] 远程执行命令
来源：http://crk.fanxiaobao.xyz

ssh user@host 'uptime'
来源：http://qxe.jianghu66.top

[R58] 下载文件
来源：http://glb.uphjek.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fsx.yanxiufei.cn

[R59] 发 POST JSON
来源：http://nok.zhijiandao.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nkp.dashuyun.cn

[R60] 只看 HTTP 状态码
来源：http://suw.shanyushiyangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://prn.feifeiyinyue.top

[R61] 磁盘占用
来源：http://jda.zdbjq.cn

df -h;  du -sh *
来源：http://nes.xuetiantiany.cn

[R62] 找最占空间的文件
来源：http://gak.tianlin.xyz

du -ah . | sort -rh | head -10
来源：http://tnp.xziqi.cn

[R63] 内存与进程
来源：http://yuk.daria6918.cn

free -h;  ps aux | grep nginx
来源：http://ztw.xziqi.cn

[R64] 结束进程
来源：http://xsc.bbcook.cn

kill -9 $(pgrep -f app.py)
来源：http://kwu.aizwys.cn

[R65] 查看端口占用
来源：http://maw.gzhubu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://syh.mhx1999.top

[R66] 定时任务
来源：http://lye.jlsjyb.cn

crontab -e;  crontab -l
来源：http://ols.0kj1m.cn

[R67] 生成随机十六进制串
来源：http://ais.redwolf501.top

openssl rand -hex 16
来源：http://vle.epnwcf.com

[R68] 计算文件校验值
来源：http://aqs.daxiang520.top

sha256sum a.txt;  md5sum a.txt
来源：http://xoc.pengpengdd.cyou

[R69] 生成随机密码
来源：http://bjv.sxryk.cn

head -c 16 /dev/urandom | base64
来源：http://nzx.9152youxi.cn

[R70] 时间戳与互转
来源：http://rib.zhiwuduotai.top

date +%s;  date -d @1700000000
来源：http://jfd.zdqjudy.top

[R71] 日期格式化
来源：http://npx.shzxlz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ymv.aibaodan.cn

[R72] 等待端口就绪
来源：http://bmd.andypj.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://apr.chenjidiqi.icu

[R73] 分割大日志
来源：http://vcb.hongshengwenyu.top

split -l 1000 big.log part_
来源：http://vtj.bbcook.cn

[R74] 批量重命名
来源：http://ydz.gotoacloud.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fhq.uphjek.com

[R75] 导出环境变量
来源：http://cgt.ydjk.org.cn

export PATH="$HOME/bin:$PATH"
来源：http://kod.hywenlv.cn

[R76] 使用临时文件
来源：http://djv.shanyushiyangtech.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tab.daxiang520.top

[R77] 读取用户输入
来源：http://bic.zhijiandao.cn

read -rp "请输入: " ans
来源：http://pgw.jianghu66.top

[R78] 交互式菜单
来源：http://zmj.uphjek.com

select opt in a b c; do echo "$opt"; break; done
来源：http://iiy.yj202588.top

[R79] 解析命令行选项
来源：http://ang.meibo888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://okz.jqgufenzy.top

[R80] 查看脚本执行耗时
来源：http://qdl.bbcook.cn

time ./run.sh
来源：http://mpk.yonumen.top

================================================================================
来源：http://tdu.xziqi.cn

S. C / C++ 专题
来源：http://tki.iojbl.cn

================================================================================
来源：http://edc.hcnkem.com

[S01] C：Hello World
来源：http://dxa.xuetiantiany.cn

#include <stdio.h>
来源：http://off.cashguo.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rnr.xinyue.icu

[S02] C：变量与格式化输出
来源：http://wzo.zdqjudy.top

int a = 10; printf("%d\n", a);
来源：http://oxa.mhx1999.top

[S03] C：读入整数
来源：http://yfd.ydjk.org.cn

int x; scanf("%d", &x);
来源：http://cke.dashuyun.cn

[S04] C：字符串复制
来源：http://eep.hysaishi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uev.tarul.cn

[S05] C：字符串长度
来源：http://ugd.xziqi.cn

strlen(s)
来源：http://pio.zhixingplan.top

[S06] C：字符串比较
来源：http://jgs.havefunace.top

strcmp(a, b) == 0
来源：http://ipx.xuanzx.com

[S07] C：数组遍历求和
来源：http://xxg.quarkkingdee.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zrt.haohaochexian.top

[S08] C：动态内存分配与释放
来源：http://wsh.sjlbkw.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lfx.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://rmj.zhijiandao.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bge.hcnkem.com

[S10] C：指针与解引用
来源：http://rxl.haohaochexian.top

int *p = &a;  *p = 5;
来源：http://mqa.jinyuanbaomall.cn

[S11] C：逐行读文件
来源：http://zff.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "r");
来源：http://cit.yonumen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://auk.ywan-chungtsiang.top

fclose(f);
来源：http://xmi.dianchejie.cn

[S12] C：写文件
来源：http://vfy.chenjidiqi.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rpc.xylfe.cn

[S13] C：宏定义
来源：http://usp.ydjk.org.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ubj.tianlin.xyz

[S14] C：枚举
来源：http://kkd.snrcjt.cn

enum Color { RED, GREEN, BLUE };
来源：http://hsv.guannengcc.top

[S15] C：类型转换
来源：http://azz.shzxlz.cn

(double) a / b
来源：http://nld.shanyushiyangkeji.top

[S16] C：位操作置位
来源：http://lgk.sweek.top

x |= (1 << 3);
来源：http://kfy.jqgfzy.top

[S17] C：安全拼接字符串
来源：http://yvs.shangyingyoupin.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qsg.shuidangran.top

[S18] C：命令行参数
来源：http://oga.shanyushiyangtech.top

int main(int argc, char **argv)
来源：http://ptj.sufxvd.cn

[S19] C：快速排序
来源：http://lqf.gzhubu.top

qsort(a, n, sizeof(int), cmp);
来源：http://kzc.tian-w.cn

[S20] C：二分查找
来源：http://rjs.52xcode.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://onq.yj20258888.top

[S21] C：字符类别判断
来源：http://yxh.chenlongwang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xka.zhoulong.xyz

[S22] C：字符串转数字
来源：http://chh.hywenlv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wzs.svipenyu.cn

[S23] C：随机数
来源：http://ura.hysaishi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hth.yj20258.top

[S24] C：获取本地时间
来源：http://obn.yj20258888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cbo.vqdsnc.cn

[S25] C：内存拷贝
来源：http://tfc.dianchejie.cn

memcpy(dst, src, n);
来源：http://apx.9152youxi.cn

[S26] C：内存清零
来源：http://dxl.bjfxy.top

memset(a, 0, sizeof a);
来源：http://uvn.jlsjyb.cn

[S27] C：定义常量
来源：http://bte.yj20258888.top

const double PI = 3.14159;
来源：http://rce.redwolf501.top

[S28] C：静态变量
来源：http://wix.jlsjyb.cn

static int counter = 0;
来源：http://eld.cashguo.top

[S29] C：变参函数
来源：http://sun.jiagoushi.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lla.zdbjq.cn

[S30] C：头文件保护
来源：http://zgs.sufxvd.cn

#ifndef X_H
来源：http://nki.hywenlv.cn

#define X_H
来源：http://bwm.hnqzz.top

#endif
来源：http://jwk.zhongyouzk.top

[S31] C++：Hello World
来源：http://lml.xingfuxueyuan.xyz

#include <iostream>
来源：http://cle.9152youxi.cn

int main() { std::cout << "Hello\n"; }
来源：http://koc.hfpthk.cn

[S32] C++：字符串
来源：http://xsr.haohaochexian.top

std::string s = "hi";  s += "!";
来源：http://vtc.yangfankeji.com

[S33] C++：vector 增删
来源：http://dqi.9152youxi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jkk.cucudq.cn

[S34] C++：遍历 vector
来源：http://ovl.chenzaomai.com

for (auto &x : v) { std::cout << x; }
来源：http://dts.snrcjt.cn


<!-- 参考信息 -->