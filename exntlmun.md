代发 wailian999

[Q76] 按天统计
来源：http://zbn.sufxvd.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://doe.fengsongda.top

[Q77] 时间加减
来源：http://kfh.wangshuangyany.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gfq.zhongyouzk.top

[Q78] 当前时间
来源：http://nwt.hcnkem.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://psd.hnqzz.top

[Q79] 字符串拼接
来源：http://xsi.snrcjt.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iep.jqgfzy.top

[Q80] 字符串截取
来源：http://zsh.ydjk.org.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gre.9152youxi.cn

[Q81] 字符串替换
来源：http://pii.jlsjyb.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mkx.yanxiufei.cn

[Q82] 字符长度与字节长度
来源：http://qhn.yonumen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fvs.yfazqb.com

[Q83] 大小写转换
来源：http://ytl.hcnkem.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://igc.sjlbkw.cn

[Q84] 去除首尾空格
来源：http://qmg.yj20258.top

SELECT TRIM(name) FROM users;
来源：http://ywa.pengpengdd.cyou

[Q85] 数值取整
来源：http://sfq.daria6918.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ril.jyoumei.cn

[Q86] 读取 JSON 字段
来源：http://bre.zdqjudy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fzk.uphjek.com

[Q87] JSON 字段做条件
来源：http://hdn.mhx1999.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dvj.tarul.cn

[Q88] 行转列（条件聚合）
来源：http://xlg.smart0.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lmh.fanxiaobao.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kuh.pengpengdd.cyou

[Q89] 判断表是否存在
来源：http://vfd.chenlongwang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://klz.yuanzhike.top

[Q90] 生成序号列
来源：http://kch.aibaodan.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pur.shanyushiyangkeji.top

================================================================================
来源：http://pgt.zhoulong.xyz

R. Bash 专题
来源：http://vfd.nanxuanxn.top

================================================================================
来源：http://fsh.shanyushiyangtech.top

[R01] shebang 与严格模式
来源：http://dli.yanxiufei.cn

#!/usr/bin/env bash
来源：http://hwk.jyoumei.cn

set -euo pipefail
来源：http://xyk.yfazqb.com

[R02] 变量赋值与使用
来源：http://ebv.guowangkeji.top

name="Tom"; echo "$name"
来源：http://eit.nwbrower.top

[R03] 只读变量
来源：http://iyt.sjlbkw.cn

readonly PI=3.14
来源：http://nvb.yj20258.top

[R04] 位置参数
来源：http://ctb.ydjk.org.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kmj.haohaochexian.top

[R05] 参数默认值
来源：http://ylp.gaohongyu789.top

name="${1:-default}"
来源：http://ptk.aibaodan.cn

[R06] 判断命令是否存在
来源：http://hpp.yangfankeji.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://frg.vqdsnc.cn

[R07] if 判断文件
来源：http://vev.iojbl.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dse.shzxlz.cn

[R08] 数值比较
来源：http://ksz.shzxlz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jjy.316326.xyz

[R09] 字符串比较
来源：http://kpr.sufxvd.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://foo.9152youxi.cn

[R10] 正则匹配
来源：http://mrt.cqqwz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://eyq.zdbjq.cn

[R11] case 多分支
来源：http://mwo.nanxinkj.top

case "$1" in
来源：http://cxd.zhixingplan.top

start) echo "启动" ;;
来源：http://esl.tian-w.cn

stop)  echo "停止" ;;
来源：http://xcf.jinyuanbaomall.cn

*)     echo "未知命令" ;;
来源：http://lho.shanyushiyangkeji.top

esac
来源：http://rid.jlsjyb.cn

[R12] for 遍历文件
来源：http://fkq.andypj.xyz

for f in *.txt; do echo "$f"; done
来源：http://aje.guannengcc.top

[R13] for 计数循环
来源：http://gue.fanxiaobao.xyz

for i in {1..10}; do echo "$i"; done
来源：http://qwp.tianlin.xyz

[R14] C 风格 for
来源：http://ehy.chenlongwang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://psz.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://vgy.gzhubu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fpp.tianlin.xyz

[R16] until 等待条件
来源：http://zgs.yj20258.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vym.mhx1999.top

[R17] 数组定义与取值
来源：http://bea.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zwb.jqgufenzy.top

[R18] 遍历数组
来源：http://oep.ppjwa.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wnr.epnwcf.com

[R19] 数组长度
来源：http://hgg.yj202588.top

echo "${#arr[@]}"
来源：http://ixv.cdnleiting.top

[R20] 关联数组（字典）
来源：http://lfz.tanke756.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bum.jqgfzy.top

[R21] 字符串长度
来源：http://guf.yfazqb.com

echo "${#s}"
来源：http://vrf.zhoulong.xyz

[R22] 截取子串
来源：http://rwt.zhoulong.xyz

echo "${s:0:5}"
来源：http://lni.havefunace.top

[R23] 字符串替换
来源：http://cqp.gaohongyu789.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dfy.52xcode.cn

[R24] 大小写转换
来源：http://oos.cheryme.top

echo "${s^^}"; echo "${s,,}"
来源：http://oqf.chenzaomai.com

[R25] 去后缀 / 去前缀
来源：http://zib.yuanzhike.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://keg.shangyingyoupin.top

[R26] 命令替换
来源：http://cfo.zdbjq.cn

now=$(date +%F); echo "$now"
来源：http://izz.guannengcc.top

[R27] 算术展开
来源：http://lhg.gzhubu.top

echo $((1 + 2 * 3))
来源：http://jij.nwbrower.top

[R28] 浮点运算
来源：http://qju.jqgfzy.top

echo "scale=2; 10/3" | bc
来源：http://ozm.bbcook.cn

[R29] 定义函数
来源：http://wty.zycfv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vsq.yueranfly.top

[R30] 函数返回状态码
来源：http://ric.birdmap.top

f() { return 0; }; f || echo "失败了"
来源：http://gfj.gogol.net.cn

[R31] 局部变量
来源：http://ide.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://rmx.yvedp.cn

[R32] 参数个数校验
来源：http://fvs.jyoumei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xsx.sxryk.cn

[R33] 捕获错误并提示行号
来源：http://fqs.shangyingyoupin.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://leg.sufxvd.cn

[R34] 退出时清理
来源：http://ojv.sweek.top

trap 'rm -f "$tmp"' EXIT
来源：http://ksf.zhaomingkeji.xyz

[R35] 后台执行并等待
来源：http://yke.daria6918.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hnr.fktsv.cn

[R36] 并发执行多个任务
来源：http://qqc.gotoacloud.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zrt.jlsjyb.cn

[R37] 把输出赋给变量
来源：http://teg.mhx1999.top

files=$(ls -1)
来源：http://zyo.fanxiaobao.xyz

[R38] 管道串联
来源：http://ess.xinyue.icu

cat a.txt | grep -i error | wc -l
来源：http://cjp.pengpengdd.cyou

[R39] 重定向标准输出与错误
来源：http://skj.quarkkingdee.top

cmd > out.log 2>&1
来源：http://shj.vqdsnc.cn

[R40] 追加写日志
来源：http://hqe.hcnkem.com

echo "log" >> out.log
来源：http://apc.hongshengwenyu.top

[R41] 丢弃输出
来源：http://udd.snrcjt.cn

cmd >/dev/null 2>&1
来源：http://bbv.316326.xyz

[R42] 输入重定向
来源：http://gnx.zhiwuduotai.top

wc -l < a.txt
来源：http://uao.wangshuangyany.cn

[R43] 按名字查找文件
来源：http://ckf.0kj1m.cn

find . -name "*.log" -type f
来源：http://aqd.hesvh.cn

[R44] 按修改时间查找
来源：http://ztq.yonumen.top

find . -mtime -7 -type f
来源：http://hbp.dianchejie.cn

[R45] 批量删除
来源：http://gin.mhx1999.top

find . -name "*.tmp" -delete
来源：http://kbk.tianlin.xyz

[R46] 递归替换文件内容
来源：http://mmk.haohaochexian.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qcd.cheryme.top

[R47] sed 单行替换
来源：http://elv.yueranfly.top

sed -i 's/foo/bar/g' a.txt
来源：http://uyj.yfazqb.com

[R48] awk 取指定列
来源：http://cae.aizwys.cn

awk '{print $1, $3}' a.txt
来源：http://rxz.tanke756.top

[R49] awk 带条件
来源：http://has.52xcode.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gzv.ppjwa.cn

[R50] awk 求和
来源：http://qwg.shanyushiyangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://qme.gzhubu.top

[R51] 排序去重取前几
来源：http://isa.yangfankeji.com

sort a.txt | uniq -c | sort -rn | head
来源：http://ihr.jqgufenzy.top

[R52] 统计行数
来源：http://loi.zhijiandao.cn

wc -l a.txt
来源：http://ihc.meibo888.top

[R53] 查看文件头与实时尾
来源：http://nvk.sweek.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fwb.yuxming.cn

[R54] 比较两个文件
来源：http://prx.zhiwuduotai.top

diff a.txt b.txt
来源：http://xme.hongshengwenyu.top

[R55] 压缩与解压
来源：http://ygd.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pag.tian-w.cn

[R56] 远程拷贝
来源：http://wji.yvedp.cn

scp file user@host:/path/
来源：http://ppb.ydzc1.top

[R57] 远程执行命令
来源：http://zgh.zycfv.cn

ssh user@host 'uptime'
来源：http://tbx.yonumen.top

[R58] 下载文件
来源：http://wjw.jinqigufen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yzs.sxryk.cn

[R59] 发 POST JSON
来源：http://ulr.cqqwz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lpu.shuidangran.top

[R60] 只看 HTTP 状态码
来源：http://ahw.zdbjq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rbj.yonumen.top

[R61] 磁盘占用
来源：http://ryg.haohaochexian.top

df -h;  du -sh *
来源：http://bqq.fzhhl.top

[R62] 找最占空间的文件
来源：http://cax.andypj.xyz

du -ah . | sort -rh | head -10
来源：http://fok.jinghuilouyu.cn

[R63] 内存与进程
来源：http://xep.jlsjyb.cn

free -h;  ps aux | grep nginx
来源：http://oqs.fanxiaobao.xyz

[R64] 结束进程
来源：http://bke.cucudq.cn

kill -9 $(pgrep -f app.py)
来源：http://izn.smart0.xyz

[R65] 查看端口占用
来源：http://trj.yanxiufei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fse.feifeiyinyue.top

[R66] 定时任务
来源：http://rfk.kuanghao11.cn

crontab -e;  crontab -l
来源：http://fiz.sysykeji.top

[R67] 生成随机十六进制串
来源：http://yqs.havefunace.top

openssl rand -hex 16
来源：http://frr.zhaomingkeji.xyz

[R68] 计算文件校验值
来源：http://lyc.zhongyouzk.top

sha256sum a.txt;  md5sum a.txt
来源：http://ktg.yuxming.cn

[R69] 生成随机密码
来源：http://mre.gogol.net.cn

head -c 16 /dev/urandom | base64
来源：http://zyg.zhaomingkeji.xyz

[R70] 时间戳与互转
来源：http://yiw.52xcode.cn

date +%s;  date -d @1700000000
来源：http://smr.fengsongda.top

[R71] 日期格式化
来源：http://etx.xziqi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uaf.yangfankeji.com

[R72] 等待端口就绪
来源：http://oip.cheryme.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bbl.yonumen.top

[R73] 分割大日志
来源：http://vlg.cashguo.top

split -l 1000 big.log part_
来源：http://bxj.ybcxt.top

[R74] 批量重命名
来源：http://ccu.sysykeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://noi.tarul.cn

[R75] 导出环境变量
来源：http://vym.havefunace.top

export PATH="$HOME/bin:$PATH"
来源：http://jtd.zycfv.cn

[R76] 使用临时文件
来源：http://cqf.hywenlv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zsl.jinyuanbaomall.cn

[R77] 读取用户输入
来源：http://ujr.hfpthk.cn

read -rp "请输入: " ans
来源：http://qca.zhixingplan.top

[R78] 交互式菜单
来源：http://lby.vehdjk.com

select opt in a b c; do echo "$opt"; break; done
来源：http://hjt.gzhubu.top

[R79] 解析命令行选项
来源：http://czh.gaohongyu789.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pqu.xingfuxueyuan.xyz

[R80] 查看脚本执行耗时
来源：http://kdk.birdmap.top

time ./run.sh
来源：http://hlb.hcnkem.com

================================================================================
来源：http://eli.shanyushiyangkeji.top

S. C / C++ 专题
来源：http://sex.feifeiyinyue.top

================================================================================
来源：http://gvj.svipenyu.cn

[S01] C：Hello World
来源：http://szm.svipenyu.cn

#include <stdio.h>
来源：http://dbw.quarkkingdee.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rbw.ppjwa.cn

[S02] C：变量与格式化输出
来源：http://obv.sweek.top

int a = 10; printf("%d\n", a);
来源：http://fjy.xuanzx.com

[S03] C：读入整数
来源：http://urt.ydjk.org.cn

int x; scanf("%d", &x);
来源：http://dte.yj20258888.top

[S04] C：字符串复制
来源：http://kuk.sjlbkw.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uan.zdbjq.cn

[S05] C：字符串长度
来源：http://wvz.iojbl.cn

strlen(s)
来源：http://eas.yangfankeji.com

[S06] C：字符串比较
来源：http://dkj.cashguo.top

strcmp(a, b) == 0
来源：http://xso.chenlongwang.top

[S07] C：数组遍历求和
来源：http://uli.smart0.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iiq.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://lvb.jyoumei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wav.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://kta.xinyue.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jsf.sjlbkw.cn

[S10] C：指针与解引用
来源：http://mob.cashguo.top

int *p = &a;  *p = 5;
来源：http://wkc.dianchejie.cn

[S11] C：逐行读文件
来源：http://roj.andypj.xyz

FILE *f = fopen("a.txt", "r");
来源：http://kpj.shangyingyoupin.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mmn.cqqwz.cn

fclose(f);
来源：http://rcw.sxryk.cn

[S12] C：写文件
来源：http://fxd.bjfxy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bob.zhijiandao.cn

[S13] C：宏定义
来源：http://tiy.hywenlv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qvq.jinghuilouyu.cn

[S14] C：枚举
来源：http://thn.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://msq.jyoumei.cn

[S15] C：类型转换
来源：http://mqh.yuanzhike.top

(double) a / b
来源：http://qow.mhx1999.top

[S16] C：位操作置位
来源：http://hhp.nanxuanxn.top

x |= (1 << 3);
来源：http://qfz.ydjk.org.cn

[S17] C：安全拼接字符串
来源：http://qsf.yj20258888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ywg.yvedp.cn

[S18] C：命令行参数
来源：http://sgh.uphjek.com

int main(int argc, char **argv)
来源：http://dxx.zhongyouzk.top

[S19] C：快速排序
来源：http://rtz.andypj.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://bvz.ehwqpu.com

[S20] C：二分查找
来源：http://izf.shuidangran.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oyd.c1oappe.top

[S21] C：字符类别判断
来源：http://eng.daria6918.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nlu.chenlongwang.top

[S22] C：字符串转数字
来源：http://hov.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://tmp.yongpay.top

[S23] C：随机数
来源：http://hzv.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://ioa.hfpthk.cn

[S24] C：获取本地时间
来源：http://gmf.cqqwz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ukf.cdnleiting.top

[S25] C：内存拷贝
来源：http://fgw.sxryk.cn

memcpy(dst, src, n);
来源：http://via.nanxuanxn.top

[S26] C：内存清零
来源：http://vro.xuanzx.com

memset(a, 0, sizeof a);
来源：http://uda.yj20258.top

[S27] C：定义常量
来源：http://mxx.ppjwa.cn

const double PI = 3.14159;
来源：http://dml.nanxuanxn.top

[S28] C：静态变量
来源：http://njl.sufxvd.cn

static int counter = 0;
来源：http://myg.cucudq.cn

[S29] C：变参函数
来源：http://tqk.pycfn.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jze.shanyushiyangtech.top

[S30] C：头文件保护
来源：http://wcf.dashuyun.cn

#ifndef X_H
来源：http://cgq.jyoumei.cn

#define X_H
来源：http://pqa.zycfv.cn

#endif
来源：http://iis.9152youxi.cn

[S31] C++：Hello World
来源：http://nnt.ehwqpu.com

#include <iostream>
来源：http://yqt.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://hgp.cqqwz.cn

[S32] C++：字符串
来源：http://uzc.yonumen.top

std::string s = "hi";  s += "!";
来源：http://cqz.kuanghao11.cn

[S33] C++：vector 增删
来源：http://bun.yj20258.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rbv.zhongyouzk.top

[S34] C++：遍历 vector
来源：http://fgm.xingfuxueyuan.xyz

for (auto &x : v) { std::cout << x; }
来源：http://ewj.zhixingplan.top

[S35] C++：map
来源：http://efw.gogol.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://edn.shuidangran.top

[S36] C++：unordered_map
来源：http://fxn.feifeiyinyue.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ilm.yj20258888.top

[S37] C++：set
来源：http://sjs.hfpthk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qxm.yj202588.top

[S38] C++：排序
来源：http://kih.andypj.xyz

std::sort(v.begin(), v.end());
来源：http://mqq.hongshengwenyu.top

[S39] C++：自定义比较器排序
来源：http://kpz.gaohongyu789.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ktf.wangdashe.top

[S40] C++：查找元素
来源：http://qtp.hywenlv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zrh.sufxvd.cn

[S41] C++：类与构造函数
来源：http://oyc.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wdq.shuidangran.top

[S42] C++：继承与虚函数
来源：http://cta.c1oappe.top

class B : public Base { public: void f() override {} };
来源：http://ufd.hfpthk.cn

[S43] C++：智能指针
来源：http://uni.yueranfly.top

auto p = std::make_unique<int>(5);
来源：http://mpt.ydzc1.top

[S44] C++：引用传参
来源：http://gok.jianghu66.top

void inc(int &x) { ++x; }
来源：http://ofu.fengsongda.top

[S45] C++：lambda
来源：http://ney.ehwqpu.com

auto add = [](int a, int b) { return a + b; };
来源：http://cdf.aizwys.cn

[S46] C++：函数模板
来源：http://ydf.tian-w.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vah.quarkkingdee.top


<!-- 参考信息 -->