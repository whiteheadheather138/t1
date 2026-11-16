代发 wailian999

ANALYZE TABLE users;
来源：http://xsf.smart0.xyz

[Q71] 查看建表语句
来源：http://fxw.zhiwuduotai.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vbx.zycfv.cn

[Q72] 查看索引
来源：http://rjc.gzhubu.top

SHOW INDEX FROM users;
来源：http://mqm.zhaomingkeji.xyz

[Q73] 查看表状态
来源：http://ouk.sxryk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dkw.jinghuilouyu.cn

[Q74] 强制使用索引
来源：http://uof.tarul.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rvs.bjfxy.top

[Q75] 日期格式化
来源：http://lbc.ivvv.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://whu.hesvh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bux.bjfxy.top

[Q76] 按天统计
来源：http://ako.shanyushiyangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://txf.feifeiyinyue.top

[Q77] 时间加减
来源：http://oin.jqgfzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wia.chenjidiqi.icu

[Q78] 当前时间
来源：http://vqt.shangyingyoupin.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xqn.hcnkem.com

[Q79] 字符串拼接
来源：http://pwa.jianghu66.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bay.redwolf501.top

[Q80] 字符串截取
来源：http://azx.zdbjq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zyz.daxiang520.top

[Q81] 字符串替换
来源：http://lih.shzxlz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wye.vehdjk.com

[Q82] 字符长度与字节长度
来源：http://ncq.shzxlz.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eqb.jlsjyb.cn

[Q83] 大小写转换
来源：http://giz.sjlbkw.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sgu.yueranfly.top

[Q84] 去除首尾空格
来源：http://hrk.zycfv.cn

SELECT TRIM(name) FROM users;
来源：http://hxb.c1oappe.top

[Q85] 数值取整
来源：http://exl.gzhubu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://izu.jianghu66.top

[Q86] 读取 JSON 字段
来源：http://bux.chenzaomai.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hmx.ywan-chungtsiang.top

[Q87] JSON 字段做条件
来源：http://oah.quarkkingdee.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://svc.pycfn.com

[Q88] 行转列（条件聚合）
来源：http://hpq.gogol.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fle.snrcjt.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://foe.wangdashe.top

[Q89] 判断表是否存在
来源：http://gna.meibo888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zdy.dashuyun.cn

[Q90] 生成序号列
来源：http://rhk.cheryme.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uti.cdnleiting.top

================================================================================
来源：http://tjq.snrcjt.cn

R. Bash 专题
来源：http://osm.tian-w.cn

================================================================================
来源：http://hjd.sysykeji.top

[R01] shebang 与严格模式
来源：http://fov.zhongyouzk.top

#!/usr/bin/env bash
来源：http://uhd.feifeiyinyue.top

set -euo pipefail
来源：http://khv.zhengqikj.top

[R02] 变量赋值与使用
来源：http://ejv.chenzaomai.com

name="Tom"; echo "$name"
来源：http://hhg.gogol.net.cn

[R03] 只读变量
来源：http://pbs.hammf.cn

readonly PI=3.14
来源：http://hin.cdnleiting.top

[R04] 位置参数
来源：http://vbn.zdqjudy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gao.52xcode.cn

[R05] 参数默认值
来源：http://pqf.hnxiangtu.top

name="${1:-default}"
来源：http://twf.tanke756.top

[R06] 判断命令是否存在
来源：http://cfi.xuetiantiany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ltm.yvedp.cn

[R07] if 判断文件
来源：http://itr.guowangkeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uul.epnwcf.com

[R08] 数值比较
来源：http://ijh.ybcxt.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pmc.xinyue.icu

[R09] 字符串比较
来源：http://tlp.xuetiantiany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lbc.guannengcc.top

[R10] 正则匹配
来源：http://vuo.dianchejie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vlo.gaohongyu789.top

[R11] case 多分支
来源：http://txs.zdqjudy.top

case "$1" in
来源：http://vzg.yuanzhike.top

start) echo "启动" ;;
来源：http://sls.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://ico.wangshuangyany.cn

*)     echo "未知命令" ;;
来源：http://rsg.vehdjk.com

esac
来源：http://dse.fehbvm.com

[R12] for 遍历文件
来源：http://jqi.jinqigufen.top

for f in *.txt; do echo "$f"; done
来源：http://yqg.tarul.cn

[R13] for 计数循环
来源：http://fww.andypj.xyz

for i in {1..10}; do echo "$i"; done
来源：http://ezw.hcnkem.com

[R14] C 风格 for
来源：http://hfu.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jdn.mhx1999.top

[R15] while 逐行读文件
来源：http://oci.jinghuilouyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lxz.xingfuxueyuan.xyz

[R16] until 等待条件
来源：http://svl.ppjwa.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gto.shzxlz.cn

[R17] 数组定义与取值
来源：http://fjs.aibaodan.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tch.haohaochexian.top

[R18] 遍历数组
来源：http://zgm.xuetiantiany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://luh.xuetiantiany.cn

[R19] 数组长度
来源：http://cav.ivvv.top

echo "${#arr[@]}"
来源：http://gqf.andypj.xyz

[R20] 关联数组（字典）
来源：http://pdp.chenjidiqi.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jcy.hywenlv.cn

[R21] 字符串长度
来源：http://vtr.zhijiandao.cn

echo "${#s}"
来源：http://zjy.cucudq.cn

[R22] 截取子串
来源：http://sfh.ywan-chungtsiang.top

echo "${s:0:5}"
来源：http://pfs.jqgfzy.top

[R23] 字符串替换
来源：http://mpq.aibaodan.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://itc.pycfn.com

[R24] 大小写转换
来源：http://ald.shanyushiyangtech.top

echo "${s^^}"; echo "${s,,}"
来源：http://ndd.aizwys.cn

[R25] 去后缀 / 去前缀
来源：http://sxy.cqqwz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qyg.daria6918.cn

[R26] 命令替换
来源：http://lxq.ppjwa.cn

now=$(date +%F); echo "$now"
来源：http://xev.yanxiufei.cn

[R27] 算术展开
来源：http://rnk.shangyingyoupin.top

echo $((1 + 2 * 3))
来源：http://ncq.vehdjk.com

[R28] 浮点运算
来源：http://mal.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://wck.sweek.top

[R29] 定义函数
来源：http://hbx.kuanghao11.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ked.jqgfzy.top

[R30] 函数返回状态码
来源：http://ajs.hysaishi.cn

f() { return 0; }; f || echo "失败了"
来源：http://oty.hysaishi.cn

[R31] 局部变量
来源：http://zmx.birdmap.top

f() { local x=1; echo "$x"; }
来源：http://yoh.sysykeji.top

[R32] 参数个数校验
来源：http://wdh.shangyingyoupin.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qxw.dashuyun.cn

[R33] 捕获错误并提示行号
来源：http://bwq.sxryk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vna.guannengcc.top

[R34] 退出时清理
来源：http://ogg.9152youxi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xww.gotoacloud.top

[R35] 后台执行并等待
来源：http://nzv.chenzaomai.com

sleep 5 & pid=$!; wait "$pid"
来源：http://zlz.hesvh.cn

[R36] 并发执行多个任务
来源：http://kxr.zhaomingkeji.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oah.shanyushiyangkeji.top

[R37] 把输出赋给变量
来源：http://pxl.xuetiantiany.cn

files=$(ls -1)
来源：http://biw.fengsongda.top

[R38] 管道串联
来源：http://bkn.ehwqpu.com

cat a.txt | grep -i error | wc -l
来源：http://pbi.jqgfzy.top

[R39] 重定向标准输出与错误
来源：http://esa.fehbvm.com

cmd > out.log 2>&1
来源：http://cus.zdqjudy.top

[R40] 追加写日志
来源：http://tos.vqdsnc.cn

echo "log" >> out.log
来源：http://tre.wangdashe.top

[R41] 丢弃输出
来源：http://vig.cashguo.top

cmd >/dev/null 2>&1
来源：http://fwt.yanxiufei.cn

[R42] 输入重定向
来源：http://snn.yueranfly.top

wc -l < a.txt
来源：http://nnh.yanxiufei.cn

[R43] 按名字查找文件
来源：http://ghp.zycfv.cn

find . -name "*.log" -type f
来源：http://rpu.jinyuanbaomall.cn

[R44] 按修改时间查找
来源：http://ezn.yongpay.top

find . -mtime -7 -type f
来源：http://frg.ehwqpu.com

[R45] 批量删除
来源：http://yrr.pycfn.com

find . -name "*.tmp" -delete
来源：http://rzt.yj20258.top

[R46] 递归替换文件内容
来源：http://kni.xuetiantiany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ztk.yongpay.top

[R47] sed 单行替换
来源：http://lor.yfazqb.com

sed -i 's/foo/bar/g' a.txt
来源：http://ani.kuanghao11.cn

[R48] awk 取指定列
来源：http://ggp.cheryme.top

awk '{print $1, $3}' a.txt
来源：http://pwv.meibo888.top

[R49] awk 带条件
来源：http://cos.9152youxi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qur.cheryme.top

[R50] awk 求和
来源：http://ayr.cheryme.top

awk '{s += $2} END {print s}' a.txt
来源：http://cmy.zhongyouzk.top

[R51] 排序去重取前几
来源：http://ngb.guowangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://deg.yj20258888.top

[R52] 统计行数
来源：http://dcc.ydzc1.top

wc -l a.txt
来源：http://qde.dashuyun.cn

[R53] 查看文件头与实时尾
来源：http://ppu.chenjidiqi.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dyh.uphjek.com

[R54] 比较两个文件
来源：http://ydm.zhixingplan.top

diff a.txt b.txt
来源：http://cma.pengpengdd.cyou

[R55] 压缩与解压
来源：http://jze.hesvh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oek.bjfxy.top

[R56] 远程拷贝
来源：http://huy.zhiwuduotai.top

scp file user@host:/path/
来源：http://por.shuidangran.top

[R57] 远程执行命令
来源：http://pym.sysykeji.top

ssh user@host 'uptime'
来源：http://smz.jiagoushi.top

[R58] 下载文件
来源：http://zqj.dashuyun.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mad.jinyuanbaomall.cn

[R59] 发 POST JSON
来源：http://wew.kuanghao11.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ehp.daxiang520.top

[R60] 只看 HTTP 状态码
来源：http://gfm.jyoumei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hhr.fktsv.cn

[R61] 磁盘占用
来源：http://xni.jinyuanbaomall.cn

df -h;  du -sh *
来源：http://uah.jinyuanbaomall.cn

[R62] 找最占空间的文件
来源：http://koy.wangdashe.top

du -ah . | sort -rh | head -10
来源：http://bvr.hammf.cn

[R63] 内存与进程
来源：http://dej.yongpay.top

free -h;  ps aux | grep nginx
来源：http://ett.yuxming.cn

[R64] 结束进程
来源：http://hlk.yangfankeji.com

kill -9 $(pgrep -f app.py)
来源：http://jjh.sysykeji.top

[R65] 查看端口占用
来源：http://aub.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ddb.ydzc1.top

[R66] 定时任务
来源：http://rkt.birdmap.top

crontab -e;  crontab -l
来源：http://vvw.gogol.net.cn

[R67] 生成随机十六进制串
来源：http://luy.quarkkingdee.top

openssl rand -hex 16
来源：http://pgv.uphjek.com

[R68] 计算文件校验值
来源：http://msn.hcnkem.com

sha256sum a.txt;  md5sum a.txt
来源：http://lga.yueranfly.top

[R69] 生成随机密码
来源：http://eop.9152youxi.cn

head -c 16 /dev/urandom | base64
来源：http://odd.hammf.cn

[R70] 时间戳与互转
来源：http://vgh.cashguo.top

date +%s;  date -d @1700000000
来源：http://bmq.xinyue.icu

[R71] 日期格式化
来源：http://tns.epnwcf.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://voa.cqqwz.cn

[R72] 等待端口就绪
来源：http://ogg.zhijiandao.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dta.ydjk.org.cn

[R73] 分割大日志
来源：http://usx.svipenyu.cn

split -l 1000 big.log part_
来源：http://nmp.xylfe.cn

[R74] 批量重命名
来源：http://xlm.haohaochexian.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xae.ivvv.top

[R75] 导出环境变量
来源：http://ccb.cheryme.top

export PATH="$HOME/bin:$PATH"
来源：http://qfz.zhiwuduotai.top

[R76] 使用临时文件
来源：http://zhf.hysaishi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bol.xuanzx.com

[R77] 读取用户输入
来源：http://svo.zhijiandao.cn

read -rp "请输入: " ans
来源：http://ycb.ppjwa.cn

[R78] 交互式菜单
来源：http://wfg.snrcjt.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bbw.cheryme.top

[R79] 解析命令行选项
来源：http://vad.tarul.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iui.cqqwz.cn

[R80] 查看脚本执行耗时
来源：http://fzw.ehwqpu.com

time ./run.sh
来源：http://hhk.smart0.xyz

================================================================================
来源：http://eak.yongpay.top

S. C / C++ 专题
来源：http://sso.cashguo.top

================================================================================
来源：http://tme.yvedp.cn

[S01] C：Hello World
来源：http://bpd.tian-w.cn

#include <stdio.h>
来源：http://fua.ydjk.org.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fyo.hnqzz.top

[S02] C：变量与格式化输出
来源：http://iio.fehbvm.com

int a = 10; printf("%d\n", a);
来源：http://zvn.havefunace.top

[S03] C：读入整数
来源：http://izf.jinqigfzy.top

int x; scanf("%d", &x);
来源：http://khi.aizwys.cn

[S04] C：字符串复制
来源：http://egx.zhoulong.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://tly.jinqigfzy.top

[S05] C：字符串长度
来源：http://cde.shangyingyoupin.top

strlen(s)
来源：http://fwj.tanke756.top

[S06] C：字符串比较
来源：http://xoe.yongpay.top

strcmp(a, b) == 0
来源：http://kjz.smart0.xyz

[S07] C：数组遍历求和
来源：http://sxn.hongshengwenyu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yld.jinghuilouyu.cn

[S08] C：动态内存分配与释放
来源：http://xhj.meibo888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zax.sjlbkw.cn

[S09] C：结构体定义与初始化
来源：http://tpr.kuanghao11.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lvd.zycfv.cn

[S10] C：指针与解引用
来源：http://udg.dianchejie.cn

int *p = &a;  *p = 5;
来源：http://ckq.cdnleiting.top

[S11] C：逐行读文件
来源：http://glq.9152youxi.cn

FILE *f = fopen("a.txt", "r");
来源：http://hyq.dianchejie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hmb.shangyingyoupin.top

fclose(f);
来源：http://yli.zhixingplan.top

[S12] C：写文件
来源：http://jxa.havefunace.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://omu.zdbjq.cn

[S13] C：宏定义
来源：http://zxg.tarul.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xmn.yongpay.top

[S14] C：枚举
来源：http://lqk.jiagoushi.top

enum Color { RED, GREEN, BLUE };
来源：http://goy.tarul.cn

[S15] C：类型转换
来源：http://vgd.xuetiantiany.cn

(double) a / b
来源：http://yat.9152youxi.cn

[S16] C：位操作置位
来源：http://sks.vehdjk.com

x |= (1 << 3);
来源：http://iwi.fengsongda.top

[S17] C：安全拼接字符串
来源：http://xel.jinqigufen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://swq.guannengcc.top

[S18] C：命令行参数
来源：http://vmb.zhiwuduotai.top

int main(int argc, char **argv)
来源：http://zom.xingfuxueyuan.xyz

[S19] C：快速排序
来源：http://rhi.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hho.xylfe.cn

[S20] C：二分查找
来源：http://mub.zhixingplan.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fmo.pycfn.com

[S21] C：字符类别判断
来源：http://cpw.ydjk.org.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eja.pycfn.com

[S22] C：字符串转数字
来源：http://vze.xuanzx.com

atoi("42");  strtod("3.14", NULL);
来源：http://xgd.yanxiufei.cn

[S23] C：随机数
来源：http://maf.quarkkingdee.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lhl.hongshengwenyu.top

[S24] C：获取本地时间
来源：http://kkf.316326.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wef.feifeiyinyue.top

[S25] C：内存拷贝
来源：http://uce.xylfe.cn

memcpy(dst, src, n);
来源：http://obs.cucudq.cn

[S26] C：内存清零
来源：http://cia.shangyingyoupin.top

memset(a, 0, sizeof a);
来源：http://uqx.ybcxt.top

[S27] C：定义常量
来源：http://egu.smart0.xyz

const double PI = 3.14159;
来源：http://zeg.jyoumei.cn

[S28] C：静态变量
来源：http://nws.jinyuanbaomall.cn

static int counter = 0;
来源：http://qxb.52xcode.cn

[S29] C：变参函数
来源：http://slc.yj20258888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bfz.jianghu66.top

[S30] C：头文件保护
来源：http://dmd.fktsv.cn

#ifndef X_H
来源：http://bvn.xuanzx.com

#define X_H
来源：http://zkj.xinyue.icu

#endif
来源：http://yvn.zdbjq.cn

[S31] C++：Hello World
来源：http://pnm.yvedp.cn

#include <iostream>
来源：http://zlf.xuetiantiany.cn

int main() { std::cout << "Hello\n"; }
来源：http://zgz.sxryk.cn

[S32] C++：字符串
来源：http://xop.shuidangran.top

std::string s = "hi";  s += "!";
来源：http://ycv.chenjidiqi.icu

[S33] C++：vector 增删
来源：http://kmh.yuanzhike.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qgc.52xcode.cn

[S34] C++：遍历 vector
来源：http://qdt.iojbl.cn

for (auto &x : v) { std::cout << x; }
来源：http://pkf.zhoulong.xyz

[S35] C++：map
来源：http://cfh.gogol.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jlb.iojbl.cn

[S36] C++：unordered_map
来源：http://chi.hnxiangtu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rwo.hesvh.cn

[S37] C++：set
来源：http://jfn.xziqi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xjd.jinghuilouyu.cn

[S38] C++：排序
来源：http://vgu.tanke756.top

std::sort(v.begin(), v.end());
来源：http://fzt.ydjk.org.cn

[S39] C++：自定义比较器排序
来源：http://tku.zdqjudy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://shr.jqgufenzy.top

[S40] C++：查找元素
来源：http://lxu.hfpthk.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xef.bjfxy.top


<!-- 参考信息 -->