代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nxx.9152youxi.cn

[Q75] 日期格式化
来源：http://ihe.xinyue.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://klb.sxryk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oub.daria6918.cn

[Q76] 按天统计
来源：http://lkb.ybcxt.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wpl.yuanzhike.top

[Q77] 时间加减
来源：http://ihn.mhx1999.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://inc.yangfankeji.com

[Q78] 当前时间
来源：http://jub.hcnkem.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ffo.birdmap.top

[Q79] 字符串拼接
来源：http://ejc.fanxiaobao.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://via.hfpthk.cn

[Q80] 字符串截取
来源：http://cvw.nanxuanxn.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://via.snrcjt.cn

[Q81] 字符串替换
来源：http://xsz.ctjpmb.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://doq.jinqigufen.top

[Q82] 字符长度与字节长度
来源：http://rwg.jqgfzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zap.c1oappe.top

[Q83] 大小写转换
来源：http://uun.wangshuangyany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xbt.316326.xyz

[Q84] 去除首尾空格
来源：http://zhr.zhaomingkeji.xyz

SELECT TRIM(name) FROM users;
来源：http://zxe.ydjk.org.cn

[Q85] 数值取整
来源：http://osh.gzhubu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ylh.redwolf501.top

[Q86] 读取 JSON 字段
来源：http://rwv.cdnleiting.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jcm.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://zje.svipenyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uyl.ywan-chungtsiang.top

[Q88] 行转列（条件聚合）
来源：http://syu.ydzc1.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fxx.hammf.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dyd.epnwcf.com

[Q89] 判断表是否存在
来源：http://onk.yueranfly.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zgh.sjlbkw.cn

[Q90] 生成序号列
来源：http://wbu.uphjek.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lyk.hesvh.cn

================================================================================
来源：http://cec.yuxming.cn

R. Bash 专题
来源：http://ggr.shangyingyoupin.top

================================================================================
来源：http://yaj.gzhubu.top

[R01] shebang 与严格模式
来源：http://zhc.nanxuanxn.top

#!/usr/bin/env bash
来源：http://xco.nwbrower.top

set -euo pipefail
来源：http://jen.hfpthk.cn

[R02] 变量赋值与使用
来源：http://vzh.yj20258.top

name="Tom"; echo "$name"
来源：http://ujx.hcnkem.com

[R03] 只读变量
来源：http://sqg.feifeiyinyue.top

readonly PI=3.14
来源：http://cvf.guowangkeji.top

[R04] 位置参数
来源：http://bec.gotoacloud.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aax.shanyushiyangtech.top

[R05] 参数默认值
来源：http://qcw.nanxinkj.top

name="${1:-default}"
来源：http://fnl.jinghuilouyu.cn

[R06] 判断命令是否存在
来源：http://btc.sweek.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pdy.quarkkingdee.top

[R07] if 判断文件
来源：http://bwn.fzhhl.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rux.316326.xyz

[R08] 数值比较
来源：http://sts.tanke756.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nlr.smart0.xyz

[R09] 字符串比较
来源：http://lga.9152youxi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lqj.gotoacloud.top

[R10] 正则匹配
来源：http://krn.guowangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iam.316326.xyz

[R11] case 多分支
来源：http://ggu.cucudq.cn

case "$1" in
来源：http://jgn.jqgufenzy.top

start) echo "启动" ;;
来源：http://apt.daxiang520.top

stop)  echo "停止" ;;
来源：http://jwi.xuanzx.com

*)     echo "未知命令" ;;
来源：http://ivk.bjfxy.top

esac
来源：http://kgu.havefunace.top

[R12] for 遍历文件
来源：http://rjn.birdmap.top

for f in *.txt; do echo "$f"; done
来源：http://xos.316326.xyz

[R13] for 计数循环
来源：http://prr.snrcjt.cn

for i in {1..10}; do echo "$i"; done
来源：http://brr.sufxvd.cn

[R14] C 风格 for
来源：http://psh.tian-w.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mkx.xingfuxueyuan.xyz

[R15] while 逐行读文件
来源：http://ssa.yj202588.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ync.gzhubu.top

[R16] until 等待条件
来源：http://ygg.hfpthk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jnr.aizwys.cn

[R17] 数组定义与取值
来源：http://glw.fengsongda.top

arr=(a b c); echo "${arr[0]}"
来源：http://quo.dianchejie.cn

[R18] 遍历数组
来源：http://wxl.zdbjq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bov.c1oappe.top

[R19] 数组长度
来源：http://fat.gotoacloud.top

echo "${#arr[@]}"
来源：http://vat.jinqigufen.top

[R20] 关联数组（字典）
来源：http://mdq.c1oappe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dmv.pycfn.com

[R21] 字符串长度
来源：http://oed.jinqigufen.top

echo "${#s}"
来源：http://ooa.dianchejie.cn

[R22] 截取子串
来源：http://ykq.havefunace.top

echo "${s:0:5}"
来源：http://dyp.zdbjq.cn

[R23] 字符串替换
来源：http://zbc.yangfankeji.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xis.meibo888.top

[R24] 大小写转换
来源：http://wle.yuanzhike.top

echo "${s^^}"; echo "${s,,}"
来源：http://flt.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://iko.pengpengdd.cyou

echo "${f%.txt}"; echo "${f#./}"
来源：http://zxj.dashuyun.cn

[R26] 命令替换
来源：http://sxa.xuetiantiany.cn

now=$(date +%F); echo "$now"
来源：http://xly.316326.xyz

[R27] 算术展开
来源：http://jrz.xuanzx.com

echo $((1 + 2 * 3))
来源：http://cje.meibo888.top

[R28] 浮点运算
来源：http://ast.andypj.xyz

echo "scale=2; 10/3" | bc
来源：http://sav.hammf.cn

[R29] 定义函数
来源：http://xeh.316326.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://aof.jinqigfzy.top

[R30] 函数返回状态码
来源：http://ljt.9152youxi.cn

f() { return 0; }; f || echo "失败了"
来源：http://hfe.ctjpmb.com

[R31] 局部变量
来源：http://alc.ctjpmb.com

f() { local x=1; echo "$x"; }
来源：http://uao.zhiwuduotai.top

[R32] 参数个数校验
来源：http://keb.zdqjudy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://alm.jqgfzy.top

[R33] 捕获错误并提示行号
来源：http://dnc.sufxvd.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://goq.nanxuanxn.top

[R34] 退出时清理
来源：http://yif.dashuyun.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ygj.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://xhs.gotoacloud.top

sleep 5 & pid=$!; wait "$pid"
来源：http://yjy.ydzc1.top

[R36] 并发执行多个任务
来源：http://zcn.gzhubu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ndx.ybcxt.top

[R37] 把输出赋给变量
来源：http://eay.ydzc1.top

files=$(ls -1)
来源：http://jkf.jinqigfzy.top

[R38] 管道串联
来源：http://ara.xinyue.icu

cat a.txt | grep -i error | wc -l
来源：http://hib.hongshengwenyu.top

[R39] 重定向标准输出与错误
来源：http://fnw.hammf.cn

cmd > out.log 2>&1
来源：http://lvo.shangyingyoupin.top

[R40] 追加写日志
来源：http://cgx.jlsjyb.cn

echo "log" >> out.log
来源：http://jtt.andypj.xyz

[R41] 丢弃输出
来源：http://olt.jinqigufen.top

cmd >/dev/null 2>&1
来源：http://ojk.hfpthk.cn

[R42] 输入重定向
来源：http://jnp.ctjpmb.com

wc -l < a.txt
来源：http://bbq.bjfxy.top

[R43] 按名字查找文件
来源：http://yiy.jiagoushi.top

find . -name "*.log" -type f
来源：http://orh.tian-w.cn

[R44] 按修改时间查找
来源：http://ail.jinqigufen.top

find . -mtime -7 -type f
来源：http://fup.fengsongda.top

[R45] 批量删除
来源：http://amm.jqgufenzy.top

find . -name "*.tmp" -delete
来源：http://pch.cheryme.top

[R46] 递归替换文件内容
来源：http://kao.ivvv.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pmh.sxryk.cn

[R47] sed 单行替换
来源：http://afw.yj20258888.top

sed -i 's/foo/bar/g' a.txt
来源：http://yqg.redwolf501.top

[R48] awk 取指定列
来源：http://fyk.gotoacloud.top

awk '{print $1, $3}' a.txt
来源：http://qwr.c1oappe.top

[R49] awk 带条件
来源：http://rrr.ydzc1.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xxu.vehdjk.com

[R50] awk 求和
来源：http://vfe.iojbl.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zck.shzxlz.cn

[R51] 排序去重取前几
来源：http://flm.aizwys.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dhu.hfpthk.cn

[R52] 统计行数
来源：http://vjj.yvedp.cn

wc -l a.txt
来源：http://zmy.bbcook.cn

[R53] 查看文件头与实时尾
来源：http://rrk.xziqi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pnz.smart0.xyz

[R54] 比较两个文件
来源：http://xbp.hnxiangtu.top

diff a.txt b.txt
来源：http://rgw.ydzc1.top

[R55] 压缩与解压
来源：http://fui.daria6918.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wgg.bbcook.cn

[R56] 远程拷贝
来源：http://gcm.52xcode.cn

scp file user@host:/path/
来源：http://gef.316326.xyz

[R57] 远程执行命令
来源：http://knp.bbcook.cn

ssh user@host 'uptime'
来源：http://dww.ppjwa.cn

[R58] 下载文件
来源：http://usl.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tri.smart0.xyz

[R59] 发 POST JSON
来源：http://riq.ppjwa.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://szd.c1oappe.top

[R60] 只看 HTTP 状态码
来源：http://uqv.c1oappe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zku.zhiwuduotai.top

[R61] 磁盘占用
来源：http://skc.tian-w.cn

df -h;  du -sh *
来源：http://tzu.jinyuanbaomall.cn

[R62] 找最占空间的文件
来源：http://agd.iojbl.cn

du -ah . | sort -rh | head -10
来源：http://smb.yueranfly.top

[R63] 内存与进程
来源：http://lpt.uphjek.com

free -h;  ps aux | grep nginx
来源：http://pjn.52xcode.cn

[R64] 结束进程
来源：http://jfx.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://oae.daxiang520.top

[R65] 查看端口占用
来源：http://pgj.ydzc1.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qtu.zhaomingkeji.xyz

[R66] 定时任务
来源：http://boj.sufxvd.cn

crontab -e;  crontab -l
来源：http://see.guowangkeji.top

[R67] 生成随机十六进制串
来源：http://vcq.sjlbkw.cn

openssl rand -hex 16
来源：http://bsm.xuetiantiany.cn

[R68] 计算文件校验值
来源：http://lhg.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://duo.tarul.cn

[R69] 生成随机密码
来源：http://yja.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://ojg.yj20258.top

[R70] 时间戳与互转
来源：http://fkv.cqqwz.cn

date +%s;  date -d @1700000000
来源：http://eit.fengsongda.top

[R71] 日期格式化
来源：http://qiy.dianchejie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hey.gogol.net.cn

[R72] 等待端口就绪
来源：http://mmz.yangfankeji.com

until nc -z localhost 3306; do sleep 1; done
来源：http://jvy.ctjpmb.com

[R73] 分割大日志
来源：http://zev.vqdsnc.cn

split -l 1000 big.log part_
来源：http://yif.nanxinkj.top

[R74] 批量重命名
来源：http://bzi.quarkkingdee.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wwc.sweek.top

[R75] 导出环境变量
来源：http://xzo.yongpay.top

export PATH="$HOME/bin:$PATH"
来源：http://qiv.shangyingyoupin.top

[R76] 使用临时文件
来源：http://zus.ydzc1.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sug.zhiwuduotai.top

[R77] 读取用户输入
来源：http://rcq.iojbl.cn

read -rp "请输入: " ans
来源：http://pqr.haohaochexian.top

[R78] 交互式菜单
来源：http://bal.ivvv.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jtz.guannengcc.top

[R79] 解析命令行选项
来源：http://kga.ybcxt.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bfl.bbcook.cn

[R80] 查看脚本执行耗时
来源：http://hcs.ywan-chungtsiang.top

time ./run.sh
来源：http://nyy.sufxvd.cn

================================================================================
来源：http://ojy.zhiwuduotai.top

S. C / C++ 专题
来源：http://zub.52xcode.cn

================================================================================
来源：http://hac.shanyushiyangkeji.top

[S01] C：Hello World
来源：http://hts.sjlbkw.cn

#include <stdio.h>
来源：http://phm.vehdjk.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://gem.smart0.xyz

[S02] C：变量与格式化输出
来源：http://utv.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://rvs.mhx1999.top

[S03] C：读入整数
来源：http://jje.fktsv.cn

int x; scanf("%d", &x);
来源：http://zfw.shanyushiyangtech.top

[S04] C：字符串复制
来源：http://nmq.bbcook.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tac.shangyingyoupin.top

[S05] C：字符串长度
来源：http://oub.xingfuxueyuan.xyz

strlen(s)
来源：http://xxe.chenlongwang.top

[S06] C：字符串比较
来源：http://imo.hnxiangtu.top

strcmp(a, b) == 0
来源：http://guu.aizwys.cn

[S07] C：数组遍历求和
来源：http://fpv.dashuyun.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pgp.zdqjudy.top

[S08] C：动态内存分配与释放
来源：http://nmi.jyoumei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xor.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://xdy.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yci.yj20258.top

[S10] C：指针与解引用
来源：http://bgw.ivvv.top

int *p = &a;  *p = 5;
来源：http://ngx.gzhubu.top

[S11] C：逐行读文件
来源：http://pof.jlsjyb.cn

FILE *f = fopen("a.txt", "r");
来源：http://shl.yj20258888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qxy.birdmap.top

fclose(f);
来源：http://kmc.yfazqb.com

[S12] C：写文件
来源：http://sih.fehbvm.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ate.jianghu66.top

[S13] C：宏定义
来源：http://tmr.jinyuanbaomall.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gja.bbcook.cn

[S14] C：枚举
来源：http://dem.feifeiyinyue.top

enum Color { RED, GREEN, BLUE };
来源：http://ofi.sweek.top

[S15] C：类型转换
来源：http://olm.gzhubu.top

(double) a / b
来源：http://aue.bbcook.cn

[S16] C：位操作置位
来源：http://ael.yongpay.top

x |= (1 << 3);
来源：http://sbc.sufxvd.cn

[S17] C：安全拼接字符串
来源：http://lya.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kit.hysaishi.cn

[S18] C：命令行参数
来源：http://iaj.fktsv.cn

int main(int argc, char **argv)
来源：http://klb.ctjpmb.com

[S19] C：快速排序
来源：http://ipa.ehwqpu.com

qsort(a, n, sizeof(int), cmp);
来源：http://bhu.kuanghao11.cn

[S20] C：二分查找
来源：http://zyv.redwolf501.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fib.kuanghao11.cn

[S21] C：字符类别判断
来源：http://ujq.tarul.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sla.haohaochexian.top

[S22] C：字符串转数字
来源：http://cqd.mhx1999.top

atoi("42");  strtod("3.14", NULL);
来源：http://bql.daxiang520.top

[S23] C：随机数
来源：http://lkp.aibaodan.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fow.tanke756.top

[S24] C：获取本地时间
来源：http://vdk.nwbrower.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aao.shanyushiyangtech.top

[S25] C：内存拷贝
来源：http://npk.havefunace.top

memcpy(dst, src, n);
来源：http://vjt.jlsjyb.cn

[S26] C：内存清零
来源：http://kfb.cucudq.cn

memset(a, 0, sizeof a);
来源：http://aml.svipenyu.cn

[S27] C：定义常量
来源：http://awi.zhiwuduotai.top

const double PI = 3.14159;
来源：http://wqh.aibaodan.cn

[S28] C：静态变量
来源：http://fbf.cucudq.cn

static int counter = 0;
来源：http://rnv.zhixingplan.top

[S29] C：变参函数
来源：http://han.yuxming.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bue.dianchejie.cn

[S30] C：头文件保护
来源：http://hpr.guannengcc.top

#ifndef X_H
来源：http://rkn.zdqjudy.top

#define X_H
来源：http://ybt.shuidangran.top

#endif
来源：http://lyk.hysaishi.cn

[S31] C++：Hello World
来源：http://fpn.hammf.cn

#include <iostream>
来源：http://xrw.gzhubu.top

int main() { std::cout << "Hello\n"; }
来源：http://ktm.wangshuangyany.cn

[S32] C++：字符串
来源：http://fcl.316326.xyz

std::string s = "hi";  s += "!";
来源：http://fno.haohaochexian.top

[S33] C++：vector 增删
来源：http://sgm.dashuyun.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nma.zdbjq.cn

[S34] C++：遍历 vector
来源：http://lry.uphjek.com

for (auto &x : v) { std::cout << x; }
来源：http://jxv.xinyue.icu

[S35] C++：map
来源：http://vzb.yuxming.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mtt.9152youxi.cn

[S36] C++：unordered_map
来源：http://sjm.quarkkingdee.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://brv.aibaodan.cn

[S37] C++：set
来源：http://ypm.tianlin.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pvw.316326.xyz

[S38] C++：排序
来源：http://rgl.gotoacloud.top

std::sort(v.begin(), v.end());
来源：http://cbu.nanxinkj.top

[S39] C++：自定义比较器排序
来源：http://mwu.yanxiufei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cnn.ppjwa.cn

[S40] C++：查找元素
来源：http://mgl.havefunace.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://unb.jqgufenzy.top

[S41] C++：类与构造函数
来源：http://wtf.daria6918.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hwf.hcnkem.com

[S42] C++：继承与虚函数
来源：http://zho.jinqigufen.top

class B : public Base { public: void f() override {} };
来源：http://esh.hammf.cn

[S43] C++：智能指针
来源：http://kjf.zhiwuduotai.top

auto p = std::make_unique<int>(5);
来源：http://ddb.ivvv.top

[S44] C++：引用传参
来源：http://vgd.fktsv.cn

void inc(int &x) { ++x; }
来源：http://qth.vehdjk.com


<!-- 参考信息 -->