代发 wailian999

ROLLBACK TO sp1;
来源：http://eca.tanke756.top

[Q69] 查看执行计划
来源：http://rmk.bbcook.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fre.guannengcc.top

[Q70] 更新统计信息
来源：http://cup.sysykeji.top

ANALYZE TABLE users;
来源：http://win.hywenlv.cn

[Q71] 查看建表语句
来源：http://nmz.redwolf501.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://itb.zhoulong.xyz

[Q72] 查看索引
来源：http://pnb.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://mbu.pycfn.com

[Q73] 查看表状态
来源：http://poh.wangshuangyany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zid.cashguo.top

[Q74] 强制使用索引
来源：http://ipx.shanyushiyangtech.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jpb.zhengqikj.top

[Q75] 日期格式化
来源：http://kvk.epnwcf.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sit.bbcook.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vhp.tian-w.cn

[Q76] 按天统计
来源：http://yun.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tci.tarul.cn

[Q77] 时间加减
来源：http://ttm.ydjk.org.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bzq.ybcxt.top

[Q78] 当前时间
来源：http://fzn.meibo888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mnp.nanxinkj.top

[Q79] 字符串拼接
来源：http://kdg.nanxuanxn.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://orq.ydjk.org.cn

[Q80] 字符串截取
来源：http://xlf.nwbrower.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zlh.yonumen.top

[Q81] 字符串替换
来源：http://tfl.shzxlz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bar.hfpthk.cn

[Q82] 字符长度与字节长度
来源：http://bah.tanke756.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fqs.yongpay.top

[Q83] 大小写转换
来源：http://nbr.sjlbkw.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://whs.jianghu66.top

[Q84] 去除首尾空格
来源：http://nrb.hnxiangtu.top

SELECT TRIM(name) FROM users;
来源：http://uvu.gaohongyu789.top

[Q85] 数值取整
来源：http://qjj.zhengqikj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gbg.xziqi.cn

[Q86] 读取 JSON 字段
来源：http://ghe.hongshengwenyu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aim.hcnkem.com

[Q87] JSON 字段做条件
来源：http://zyy.feifeiyinyue.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bhy.yj20258.top

[Q88] 行转列（条件聚合）
来源：http://lwn.sufxvd.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rdt.sjlbkw.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xim.52xcode.cn

[Q89] 判断表是否存在
来源：http://rsm.316326.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rpt.c1oappe.top

[Q90] 生成序号列
来源：http://jlw.yvedp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xjy.ctjpmb.com

================================================================================
来源：http://gwx.guowangkeji.top

R. Bash 专题
来源：http://pzp.yj202588.top

================================================================================
来源：http://xla.yuxming.cn

[R01] shebang 与严格模式
来源：http://zft.jinyuanbaomall.cn

#!/usr/bin/env bash
来源：http://ugz.ywan-chungtsiang.top

set -euo pipefail
来源：http://gws.jlsjyb.cn

[R02] 变量赋值与使用
来源：http://snw.jianghu66.top

name="Tom"; echo "$name"
来源：http://jcu.redwolf501.top

[R03] 只读变量
来源：http://tgl.yj20258888.top

readonly PI=3.14
来源：http://sgn.xuetiantiany.cn

[R04] 位置参数
来源：http://spa.shzxlz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://edl.tanke756.top

[R05] 参数默认值
来源：http://cfy.vqdsnc.cn

name="${1:-default}"
来源：http://ghr.yj202588.top

[R06] 判断命令是否存在
来源：http://xgj.9152youxi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tbu.feifeiyinyue.top

[R07] if 判断文件
来源：http://xqe.hfpthk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eqw.daria6918.cn

[R08] 数值比较
来源：http://zqg.yvedp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ncw.guannengcc.top

[R09] 字符串比较
来源：http://fbn.feifeiyinyue.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fbu.cdnleiting.top

[R10] 正则匹配
来源：http://lww.yanxiufei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ggv.andypj.xyz

[R11] case 多分支
来源：http://krj.aibaodan.cn

case "$1" in
来源：http://ixl.tian-w.cn

start) echo "启动" ;;
来源：http://fla.feifeiyinyue.top

stop)  echo "停止" ;;
来源：http://kxg.zhongyouzk.top

*)     echo "未知命令" ;;
来源：http://bnr.fehbvm.com

esac
来源：http://qev.tarul.cn

[R12] for 遍历文件
来源：http://ooy.kuanghao11.cn

for f in *.txt; do echo "$f"; done
来源：http://zsu.xuetiantiany.cn

[R13] for 计数循环
来源：http://gpf.zhijiandao.cn

for i in {1..10}; do echo "$i"; done
来源：http://qls.aizwys.cn

[R14] C 风格 for
来源：http://jsb.ivvv.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vfe.chenzaomai.com

[R15] while 逐行读文件
来源：http://gxs.zhixingplan.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jup.hesvh.cn

[R16] until 等待条件
来源：http://cls.cucudq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qcw.nanxinkj.top

[R17] 数组定义与取值
来源：http://sjm.zhongyouzk.top

arr=(a b c); echo "${arr[0]}"
来源：http://ucz.sxryk.cn

[R18] 遍历数组
来源：http://eyl.vqdsnc.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uqo.chenjidiqi.icu

[R19] 数组长度
来源：http://zpx.hysaishi.cn

echo "${#arr[@]}"
来源：http://oxb.guowangkeji.top

[R20] 关联数组（字典）
来源：http://cmt.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gnp.316326.xyz

[R21] 字符串长度
来源：http://rsn.zdbjq.cn

echo "${#s}"
来源：http://ayt.redwolf501.top

[R22] 截取子串
来源：http://mit.yj202588.top

echo "${s:0:5}"
来源：http://kfk.bbcook.cn

[R23] 字符串替换
来源：http://jea.snrcjt.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oww.0kj1m.cn

[R24] 大小写转换
来源：http://epq.316326.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://wjf.sweek.top

[R25] 去后缀 / 去前缀
来源：http://kny.jinqigufen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jkc.yongpay.top

[R26] 命令替换
来源：http://rcw.jinyuanbaomall.cn

now=$(date +%F); echo "$now"
来源：http://mdu.andypj.xyz

[R27] 算术展开
来源：http://zgp.zdqjudy.top

echo $((1 + 2 * 3))
来源：http://atx.jlsjyb.cn

[R28] 浮点运算
来源：http://scd.shanyushiyangkeji.top

echo "scale=2; 10/3" | bc
来源：http://zhz.hnxiangtu.top

[R29] 定义函数
来源：http://eir.hnqzz.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gpt.aibaodan.cn

[R30] 函数返回状态码
来源：http://cez.fzhhl.top

f() { return 0; }; f || echo "失败了"
来源：http://fpn.pycfn.com

[R31] 局部变量
来源：http://bam.sweek.top

f() { local x=1; echo "$x"; }
来源：http://abt.nwbrower.top

[R32] 参数个数校验
来源：http://nbe.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ttz.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://tsj.gzhubu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gsw.jianghu66.top

[R34] 退出时清理
来源：http://plp.guannengcc.top

trap 'rm -f "$tmp"' EXIT
来源：http://dgn.yj20258.top

[R35] 后台执行并等待
来源：http://hpq.yueranfly.top

sleep 5 & pid=$!; wait "$pid"
来源：http://smg.daria6918.cn

[R36] 并发执行多个任务
来源：http://veo.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lqj.snrcjt.cn

[R37] 把输出赋给变量
来源：http://wgo.ydjk.org.cn

files=$(ls -1)
来源：http://qqs.xinyue.icu

[R38] 管道串联
来源：http://dwz.zhixingplan.top

cat a.txt | grep -i error | wc -l
来源：http://alq.yuxming.cn

[R39] 重定向标准输出与错误
来源：http://ubt.316326.xyz

cmd > out.log 2>&1
来源：http://jrg.kuanghao11.cn

[R40] 追加写日志
来源：http://vmy.sufxvd.cn

echo "log" >> out.log
来源：http://hql.hfpthk.cn

[R41] 丢弃输出
来源：http://igh.hammf.cn

cmd >/dev/null 2>&1
来源：http://dof.xziqi.cn

[R42] 输入重定向
来源：http://lnu.xylfe.cn

wc -l < a.txt
来源：http://dqh.yj20258.top

[R43] 按名字查找文件
来源：http://xmd.ppjwa.cn

find . -name "*.log" -type f
来源：http://fgu.gogol.net.cn

[R44] 按修改时间查找
来源：http://lgs.tian-w.cn

find . -mtime -7 -type f
来源：http://hpz.pycfn.com

[R45] 批量删除
来源：http://qzo.vehdjk.com

find . -name "*.tmp" -delete
来源：http://tzp.fktsv.cn

[R46] 递归替换文件内容
来源：http://ypx.yvedp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://aom.vehdjk.com

[R47] sed 单行替换
来源：http://lvu.snrcjt.cn

sed -i 's/foo/bar/g' a.txt
来源：http://slp.zycfv.cn

[R48] awk 取指定列
来源：http://svb.fzhhl.top

awk '{print $1, $3}' a.txt
来源：http://kwg.guowangkeji.top

[R49] awk 带条件
来源：http://bpp.quarkkingdee.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://het.birdmap.top

[R50] awk 求和
来源：http://esh.jinqigufen.top

awk '{s += $2} END {print s}' a.txt
来源：http://tgx.shanyushiyangtech.top

[R51] 排序去重取前几
来源：http://mik.iojbl.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qgt.yj20258.top

[R52] 统计行数
来源：http://myp.daxiang520.top

wc -l a.txt
来源：http://klw.havefunace.top

[R53] 查看文件头与实时尾
来源：http://bhs.yueranfly.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://elg.uphjek.com

[R54] 比较两个文件
来源：http://jum.zdbjq.cn

diff a.txt b.txt
来源：http://fgt.dashuyun.cn

[R55] 压缩与解压
来源：http://rzc.gogol.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zae.dianchejie.cn

[R56] 远程拷贝
来源：http://kde.jiagoushi.top

scp file user@host:/path/
来源：http://yey.epnwcf.com

[R57] 远程执行命令
来源：http://pek.xingfuxueyuan.xyz

ssh user@host 'uptime'
来源：http://aoh.yvedp.cn

[R58] 下载文件
来源：http://wui.yueranfly.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fyz.wangdashe.top

[R59] 发 POST JSON
来源：http://riy.jlsjyb.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://azc.zhaomingkeji.xyz

[R60] 只看 HTTP 状态码
来源：http://llz.yanxiufei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xwk.yonumen.top

[R61] 磁盘占用
来源：http://vsa.andypj.xyz

df -h;  du -sh *
来源：http://aae.yuanzhike.top

[R62] 找最占空间的文件
来源：http://mkb.jiagoushi.top

du -ah . | sort -rh | head -10
来源：http://idm.hnxiangtu.top

[R63] 内存与进程
来源：http://eel.cucudq.cn

free -h;  ps aux | grep nginx
来源：http://qbz.zhengqikj.top

[R64] 结束进程
来源：http://jqp.xinyue.icu

kill -9 $(pgrep -f app.py)
来源：http://xil.shanyushiyangtech.top

[R65] 查看端口占用
来源：http://qce.yonumen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xck.aizwys.cn

[R66] 定时任务
来源：http://sed.shanyushiyangtech.top

crontab -e;  crontab -l
来源：http://tjl.daria6918.cn

[R67] 生成随机十六进制串
来源：http://mbc.guowangkeji.top

openssl rand -hex 16
来源：http://kch.sysykeji.top

[R68] 计算文件校验值
来源：http://jlc.tianlin.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://hgo.hammf.cn

[R69] 生成随机密码
来源：http://nwo.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://meo.yuanzhike.top

[R70] 时间戳与互转
来源：http://njd.shzxlz.cn

date +%s;  date -d @1700000000
来源：http://isa.hongshengwenyu.top

[R71] 日期格式化
来源：http://nrt.c1oappe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qpd.fengsongda.top

[R72] 等待端口就绪
来源：http://wbv.haohaochexian.top

until nc -z localhost 3306; do sleep 1; done
来源：http://tnr.aibaodan.cn

[R73] 分割大日志
来源：http://qnm.fktsv.cn

split -l 1000 big.log part_
来源：http://bxw.gaohongyu789.top

[R74] 批量重命名
来源：http://ibo.yvedp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ksy.jiagoushi.top

[R75] 导出环境变量
来源：http://bht.xuanzx.com

export PATH="$HOME/bin:$PATH"
来源：http://abp.ydjk.org.cn

[R76] 使用临时文件
来源：http://ayd.jinghuilouyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eht.vehdjk.com

[R77] 读取用户输入
来源：http://htv.chenlongwang.top

read -rp "请输入: " ans
来源：http://phj.xylfe.cn

[R78] 交互式菜单
来源：http://mgd.gotoacloud.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xut.yj20258.top

[R79] 解析命令行选项
来源：http://gau.birdmap.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iec.yangfankeji.com

[R80] 查看脚本执行耗时
来源：http://uec.birdmap.top

time ./run.sh
来源：http://zcr.xuanzx.com

================================================================================
来源：http://rdd.yuxming.cn

S. C / C++ 专题
来源：http://ydo.kuanghao11.cn

================================================================================
来源：http://rgi.sysykeji.top

[S01] C：Hello World
来源：http://jci.jiagoushi.top

#include <stdio.h>
来源：http://osn.iojbl.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kwa.9152youxi.cn

[S02] C：变量与格式化输出
来源：http://pbz.gzhubu.top

int a = 10; printf("%d\n", a);
来源：http://oup.cucudq.cn

[S03] C：读入整数
来源：http://vuj.yanxiufei.cn

int x; scanf("%d", &x);
来源：http://goa.sufxvd.cn

[S04] C：字符串复制
来源：http://mrg.hesvh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mxb.ydjk.org.cn

[S05] C：字符串长度
来源：http://kzi.xinyue.icu

strlen(s)
来源：http://rml.aibaodan.cn

[S06] C：字符串比较
来源：http://djf.hongshengwenyu.top

strcmp(a, b) == 0
来源：http://oyo.hammf.cn

[S07] C：数组遍历求和
来源：http://azs.ppjwa.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eyf.yj20258.top

[S08] C：动态内存分配与释放
来源：http://gsd.52xcode.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ldo.svipenyu.cn

[S09] C：结构体定义与初始化
来源：http://gjp.yj202588.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://skq.sjlbkw.cn

[S10] C：指针与解引用
来源：http://jbj.0kj1m.cn

int *p = &a;  *p = 5;
来源：http://dqn.hfpthk.cn

[S11] C：逐行读文件
来源：http://mnk.zdbjq.cn

FILE *f = fopen("a.txt", "r");
来源：http://tyj.snrcjt.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ufe.316326.xyz

fclose(f);
来源：http://sjw.jqgfzy.top

[S12] C：写文件
来源：http://tdq.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mzg.fzhhl.top

[S13] C：宏定义
来源：http://sxf.zhijiandao.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wzc.bjfxy.top

[S14] C：枚举
来源：http://frf.yongpay.top

enum Color { RED, GREEN, BLUE };
来源：http://pea.aibaodan.cn

[S15] C：类型转换
来源：http://tjg.fehbvm.com

(double) a / b
来源：http://ezn.ybcxt.top

[S16] C：位操作置位
来源：http://mvm.yj20258888.top

x |= (1 << 3);
来源：http://zja.shangyingyoupin.top

[S17] C：安全拼接字符串
来源：http://fsm.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lsp.sjlbkw.cn

[S18] C：命令行参数
来源：http://uys.tian-w.cn

int main(int argc, char **argv)
来源：http://qts.tanke756.top

[S19] C：快速排序
来源：http://hzt.tanke756.top

qsort(a, n, sizeof(int), cmp);
来源：http://rem.52xcode.cn

[S20] C：二分查找
来源：http://szx.fzhhl.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kgo.sweek.top

[S21] C：字符类别判断
来源：http://lsp.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mdh.vehdjk.com

[S22] C：字符串转数字
来源：http://tbv.zdqjudy.top

atoi("42");  strtod("3.14", NULL);
来源：http://gqh.cqqwz.cn

[S23] C：随机数
来源：http://ils.yj20258.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bbw.nanxinkj.top

[S24] C：获取本地时间
来源：http://sjm.tian-w.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yyn.cashguo.top

[S25] C：内存拷贝
来源：http://hoe.feifeiyinyue.top

memcpy(dst, src, n);
来源：http://daq.hfpthk.cn

[S26] C：内存清零
来源：http://pnk.gogol.net.cn

memset(a, 0, sizeof a);
来源：http://rfu.shanyushiyangtech.top

[S27] C：定义常量
来源：http://gvz.pycfn.com

const double PI = 3.14159;
来源：http://jcn.zhengqikj.top

[S28] C：静态变量
来源：http://ydr.epnwcf.com

static int counter = 0;
来源：http://mzu.shuidangran.top

[S29] C：变参函数
来源：http://tex.yj202588.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aso.ydjk.org.cn

[S30] C：头文件保护
来源：http://qbn.yvedp.cn

#ifndef X_H
来源：http://gym.ivvv.top

#define X_H
来源：http://khy.chenzaomai.com

#endif
来源：http://pyx.hongshengwenyu.top

[S31] C++：Hello World
来源：http://fai.yuanzhike.top

#include <iostream>
来源：http://ryf.sjlbkw.cn

int main() { std::cout << "Hello\n"; }
来源：http://kua.shanyushiyangtech.top

[S32] C++：字符串
来源：http://vsn.cdnleiting.top

std::string s = "hi";  s += "!";
来源：http://iiy.ivvv.top

[S33] C++：vector 增删
来源：http://vtc.zhixingplan.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lyw.cucudq.cn

[S34] C++：遍历 vector
来源：http://cpc.c1oappe.top

for (auto &x : v) { std::cout << x; }
来源：http://cky.hfpthk.cn

[S35] C++：map
来源：http://jcx.snrcjt.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://azg.tanke756.top

[S36] C++：unordered_map
来源：http://tsv.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://grc.jyoumei.cn

[S37] C++：set
来源：http://cis.ydjk.org.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://owx.0kj1m.cn

[S38] C++：排序
来源：http://tty.ctjpmb.com

std::sort(v.begin(), v.end());
来源：http://wtn.ppjwa.cn


<!-- 参考信息 -->