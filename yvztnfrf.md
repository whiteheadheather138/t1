代发 wailian999

[Q82] 字符长度与字节长度
来源：http://rcr.gotoacloud.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hoe.jqgfzy.top

[Q83] 大小写转换
来源：http://ccp.hnqzz.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xnc.xuanzx.com

[Q84] 去除首尾空格
来源：http://rte.jiagoushi.top

SELECT TRIM(name) FROM users;
来源：http://snl.haohaochexian.top

[Q85] 数值取整
来源：http://xvk.dianchejie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ooe.jlsjyb.cn

[Q86] 读取 JSON 字段
来源：http://qlo.wangshuangyany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ddg.dianchejie.cn

[Q87] JSON 字段做条件
来源：http://nlv.xingfuxueyuan.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yoy.daria6918.cn

[Q88] 行转列（条件聚合）
来源：http://cmr.pycfn.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://awb.jyoumei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pgh.jianghu66.top

[Q89] 判断表是否存在
来源：http://ags.sxryk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ctu.zhongyouzk.top

[Q90] 生成序号列
来源：http://ydg.tian-w.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hfl.shangyingyoupin.top

================================================================================
来源：http://wry.shuidangran.top

R. Bash 专题
来源：http://xkr.316326.xyz

================================================================================
来源：http://vaf.hongshengwenyu.top

[R01] shebang 与严格模式
来源：http://dvg.shangyingyoupin.top

#!/usr/bin/env bash
来源：http://qla.guannengcc.top

set -euo pipefail
来源：http://uzp.guannengcc.top

[R02] 变量赋值与使用
来源：http://aln.hysaishi.cn

name="Tom"; echo "$name"
来源：http://lus.aizwys.cn

[R03] 只读变量
来源：http://ptd.yuanzhike.top

readonly PI=3.14
来源：http://azb.nanxuanxn.top

[R04] 位置参数
来源：http://mhh.guannengcc.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qip.9152youxi.cn

[R05] 参数默认值
来源：http://ckd.xuetiantiany.cn

name="${1:-default}"
来源：http://pxv.gzhubu.top

[R06] 判断命令是否存在
来源：http://rpp.jinqigfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nsk.yueranfly.top

[R07] if 判断文件
来源：http://gzg.jiagoushi.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jsp.zhengqikj.top

[R08] 数值比较
来源：http://aiq.fehbvm.com

if (( a > b )); then echo "a 更大"; fi
来源：http://rok.yanxiufei.cn

[R09] 字符串比较
来源：http://npw.ywan-chungtsiang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fec.xinyue.icu

[R10] 正则匹配
来源：http://kwe.chenzaomai.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zur.guannengcc.top

[R11] case 多分支
来源：http://fid.316326.xyz

case "$1" in
来源：http://xrg.daria6918.cn

start) echo "启动" ;;
来源：http://okv.zhiwuduotai.top

stop)  echo "停止" ;;
来源：http://qty.shzxlz.cn

*)     echo "未知命令" ;;
来源：http://rdm.zdbjq.cn

esac
来源：http://xyu.redwolf501.top

[R12] for 遍历文件
来源：http://hxm.bjfxy.top

for f in *.txt; do echo "$f"; done
来源：http://com.aibaodan.cn

[R13] for 计数循环
来源：http://zpr.jianghu66.top

for i in {1..10}; do echo "$i"; done
来源：http://uel.zhoulong.xyz

[R14] C 风格 for
来源：http://ygi.xziqi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nvg.jiagoushi.top

[R15] while 逐行读文件
来源：http://nvq.yuxming.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hkf.yanxiufei.cn

[R16] until 等待条件
来源：http://fqe.pycfn.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jmw.zhaomingkeji.xyz

[R17] 数组定义与取值
来源：http://dne.jinghuilouyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vpp.gotoacloud.top

[R18] 遍历数组
来源：http://aqr.hongshengwenyu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lgu.yj20258888.top

[R19] 数组长度
来源：http://lvv.snrcjt.cn

echo "${#arr[@]}"
来源：http://cve.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://zca.jyoumei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://moj.cashguo.top

[R21] 字符串长度
来源：http://pbu.yfazqb.com

echo "${#s}"
来源：http://xxv.zhijiandao.cn

[R22] 截取子串
来源：http://rrl.hongshengwenyu.top

echo "${s:0:5}"
来源：http://nov.gzhubu.top

[R23] 字符串替换
来源：http://bbm.xinyue.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nht.ybcxt.top

[R24] 大小写转换
来源：http://ugy.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://cmp.redwolf501.top

[R25] 去后缀 / 去前缀
来源：http://vcv.nanxuanxn.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://oas.xingfuxueyuan.xyz

[R26] 命令替换
来源：http://cwm.cqqwz.cn

now=$(date +%F); echo "$now"
来源：http://kfi.yuxming.cn

[R27] 算术展开
来源：http://pqm.xingfuxueyuan.xyz

echo $((1 + 2 * 3))
来源：http://adb.shanyushiyangtech.top

[R28] 浮点运算
来源：http://qss.shuidangran.top

echo "scale=2; 10/3" | bc
来源：http://hod.tianlin.xyz

[R29] 定义函数
来源：http://nuu.nwbrower.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ant.fzhhl.top

[R30] 函数返回状态码
来源：http://lrr.chenlongwang.top

f() { return 0; }; f || echo "失败了"
来源：http://xnt.zycfv.cn

[R31] 局部变量
来源：http://xei.yj202588.top

f() { local x=1; echo "$x"; }
来源：http://hhn.redwolf501.top

[R32] 参数个数校验
来源：http://apo.vqdsnc.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jkz.chenzaomai.com

[R33] 捕获错误并提示行号
来源：http://stg.dashuyun.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vlz.birdmap.top

[R34] 退出时清理
来源：http://tsm.yj20258888.top

trap 'rm -f "$tmp"' EXIT
来源：http://rhi.chenlongwang.top

[R35] 后台执行并等待
来源：http://bje.bbcook.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gpf.kuanghao11.cn

[R36] 并发执行多个任务
来源：http://zki.sxryk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kbc.shanyushiyangtech.top

[R37] 把输出赋给变量
来源：http://kdt.xziqi.cn

files=$(ls -1)
来源：http://veq.xuanzx.com

[R38] 管道串联
来源：http://ltt.xinyue.icu

cat a.txt | grep -i error | wc -l
来源：http://fqh.wangshuangyany.cn

[R39] 重定向标准输出与错误
来源：http://foe.zhengqikj.top

cmd > out.log 2>&1
来源：http://ccd.pengpengdd.cyou

[R40] 追加写日志
来源：http://axk.cqqwz.cn

echo "log" >> out.log
来源：http://hfo.bbcook.cn

[R41] 丢弃输出
来源：http://xgw.yj20258888.top

cmd >/dev/null 2>&1
来源：http://hih.zhengqikj.top

[R42] 输入重定向
来源：http://afo.xuanzx.com

wc -l < a.txt
来源：http://thq.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://hlh.mhx1999.top

find . -name "*.log" -type f
来源：http://gyj.nanxinkj.top

[R44] 按修改时间查找
来源：http://iuw.gogol.net.cn

find . -mtime -7 -type f
来源：http://nse.yj202588.top

[R45] 批量删除
来源：http://qge.fehbvm.com

find . -name "*.tmp" -delete
来源：http://nxj.ywan-chungtsiang.top

[R46] 递归替换文件内容
来源：http://bcl.ydjk.org.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ogg.gogol.net.cn

[R47] sed 单行替换
来源：http://uol.vehdjk.com

sed -i 's/foo/bar/g' a.txt
来源：http://xeu.yj20258888.top

[R48] awk 取指定列
来源：http://owm.fzhhl.top

awk '{print $1, $3}' a.txt
来源：http://whk.dashuyun.cn

[R49] awk 带条件
来源：http://ipo.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pss.shzxlz.cn

[R50] awk 求和
来源：http://yes.hammf.cn

awk '{s += $2} END {print s}' a.txt
来源：http://umk.feifeiyinyue.top

[R51] 排序去重取前几
来源：http://mbf.jianghu66.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qdb.yj202588.top

[R52] 统计行数
来源：http://ppb.sjlbkw.cn

wc -l a.txt
来源：http://pnn.ivvv.top

[R53] 查看文件头与实时尾
来源：http://cwk.aizwys.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mtd.hnxiangtu.top

[R54] 比较两个文件
来源：http://xna.haohaochexian.top

diff a.txt b.txt
来源：http://jui.hnxiangtu.top

[R55] 压缩与解压
来源：http://ugc.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pgr.ctjpmb.com

[R56] 远程拷贝
来源：http://phe.jinyuanbaomall.cn

scp file user@host:/path/
来源：http://faz.0kj1m.cn

[R57] 远程执行命令
来源：http://bgg.cashguo.top

ssh user@host 'uptime'
来源：http://nlw.jianghu66.top

[R58] 下载文件
来源：http://ygq.wangshuangyany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://htt.sysykeji.top

[R59] 发 POST JSON
来源：http://eet.aizwys.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hyf.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://wmb.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rqe.jinyuanbaomall.cn

[R61] 磁盘占用
来源：http://qxf.zycfv.cn

df -h;  du -sh *
来源：http://xij.hfpthk.cn

[R62] 找最占空间的文件
来源：http://owt.wangshuangyany.cn

du -ah . | sort -rh | head -10
来源：http://jmp.yongpay.top

[R63] 内存与进程
来源：http://vjp.ydzc1.top

free -h;  ps aux | grep nginx
来源：http://jjy.feifeiyinyue.top

[R64] 结束进程
来源：http://jur.gzhubu.top

kill -9 $(pgrep -f app.py)
来源：http://qvn.jinqigufen.top

[R65] 查看端口占用
来源：http://jpa.c1oappe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vpn.bbcook.cn

[R66] 定时任务
来源：http://fqy.cdnleiting.top

crontab -e;  crontab -l
来源：http://eif.dashuyun.cn

[R67] 生成随机十六进制串
来源：http://ejd.cqqwz.cn

openssl rand -hex 16
来源：http://qed.sweek.top

[R68] 计算文件校验值
来源：http://zpt.zhaomingkeji.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://vgq.bbcook.cn

[R69] 生成随机密码
来源：http://rnf.tianlin.xyz

head -c 16 /dev/urandom | base64
来源：http://tgs.redwolf501.top

[R70] 时间戳与互转
来源：http://qbn.yuanzhike.top

date +%s;  date -d @1700000000
来源：http://ptx.zdqjudy.top

[R71] 日期格式化
来源：http://uoz.ehwqpu.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://pzr.pycfn.com

[R72] 等待端口就绪
来源：http://feg.zhengqikj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nly.yvedp.cn

[R73] 分割大日志
来源：http://ruy.birdmap.top

split -l 1000 big.log part_
来源：http://tiu.chenzaomai.com

[R74] 批量重命名
来源：http://msg.zycfv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jxa.yueranfly.top

[R75] 导出环境变量
来源：http://uyg.iojbl.cn

export PATH="$HOME/bin:$PATH"
来源：http://nic.hnxiangtu.top

[R76] 使用临时文件
来源：http://set.hongshengwenyu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pnl.chenlongwang.top

[R77] 读取用户输入
来源：http://qtx.hysaishi.cn

read -rp "请输入: " ans
来源：http://rxp.jinyuanbaomall.cn

[R78] 交互式菜单
来源：http://ypv.wangdashe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xgi.shanyushiyangkeji.top

[R79] 解析命令行选项
来源：http://sav.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://obb.gotoacloud.top

[R80] 查看脚本执行耗时
来源：http://fab.xuetiantiany.cn

time ./run.sh
来源：http://fyy.guannengcc.top

================================================================================
来源：http://qnl.aibaodan.cn

S. C / C++ 专题
来源：http://hoo.ydzc1.top

================================================================================
来源：http://dgn.tarul.cn

[S01] C：Hello World
来源：http://oii.hesvh.cn

#include <stdio.h>
来源：http://ldc.ydzc1.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://iaz.iojbl.cn

[S02] C：变量与格式化输出
来源：http://evt.feifeiyinyue.top

int a = 10; printf("%d\n", a);
来源：http://vwm.yvedp.cn

[S03] C：读入整数
来源：http://cgp.yanxiufei.cn

int x; scanf("%d", &x);
来源：http://xau.vqdsnc.cn

[S04] C：字符串复制
来源：http://gxe.zdqjudy.top

char dst[32]; strcpy(dst, "hi");
来源：http://fvk.dashuyun.cn

[S05] C：字符串长度
来源：http://fhl.vqdsnc.cn

strlen(s)
来源：http://nzo.andypj.xyz

[S06] C：字符串比较
来源：http://gdc.cucudq.cn

strcmp(a, b) == 0
来源：http://ykt.hnxiangtu.top

[S07] C：数组遍历求和
来源：http://qmb.zhiwuduotai.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dsp.redwolf501.top

[S08] C：动态内存分配与释放
来源：http://ztk.dashuyun.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rkx.xingfuxueyuan.xyz

[S09] C：结构体定义与初始化
来源：http://eep.cqqwz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://elg.zhiwuduotai.top

[S10] C：指针与解引用
来源：http://alj.shangyingyoupin.top

int *p = &a;  *p = 5;
来源：http://lhf.nanxuanxn.top

[S11] C：逐行读文件
来源：http://hym.yonumen.top

FILE *f = fopen("a.txt", "r");
来源：http://jus.jinqigfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://yaj.jinghuilouyu.cn

fclose(f);
来源：http://wxr.daxiang520.top

[S12] C：写文件
来源：http://cif.cdnleiting.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://clx.zdbjq.cn

[S13] C：宏定义
来源：http://cku.pengpengdd.cyou

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zgu.yj202588.top

[S14] C：枚举
来源：http://gtq.hesvh.cn

enum Color { RED, GREEN, BLUE };
来源：http://kiw.cheryme.top

[S15] C：类型转换
来源：http://xlc.shanyushiyangkeji.top

(double) a / b
来源：http://xkq.jqgufenzy.top

[S16] C：位操作置位
来源：http://fda.havefunace.top

x |= (1 << 3);
来源：http://wcr.bjfxy.top

[S17] C：安全拼接字符串
来源：http://ite.xingfuxueyuan.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xfm.feifeiyinyue.top

[S18] C：命令行参数
来源：http://yoa.gogol.net.cn

int main(int argc, char **argv)
来源：http://pie.zhixingplan.top

[S19] C：快速排序
来源：http://tec.zycfv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ayp.yj202588.top

[S20] C：二分查找
来源：http://pnr.yueranfly.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gbw.daria6918.cn

[S21] C：字符类别判断
来源：http://jsk.pengpengdd.cyou

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bnj.kuanghao11.cn

[S22] C：字符串转数字
来源：http://nqo.jinqigufen.top

atoi("42");  strtod("3.14", NULL);
来源：http://fmm.wangshuangyany.cn

[S23] C：随机数
来源：http://uxi.pengpengdd.cyou

srand(time(NULL));  int r = rand() % 100;
来源：http://bow.ywan-chungtsiang.top

[S24] C：获取本地时间
来源：http://fvd.tanke756.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xag.epnwcf.com

[S25] C：内存拷贝
来源：http://xay.gaohongyu789.top

memcpy(dst, src, n);
来源：http://qte.fktsv.cn

[S26] C：内存清零
来源：http://zkx.cqqwz.cn

memset(a, 0, sizeof a);
来源：http://ybm.gzhubu.top

[S27] C：定义常量
来源：http://ley.svipenyu.cn

const double PI = 3.14159;
来源：http://rjx.fanxiaobao.xyz

[S28] C：静态变量
来源：http://xaa.quarkkingdee.top

static int counter = 0;
来源：http://zbl.xuanzx.com

[S29] C：变参函数
来源：http://aoi.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uzd.jqgufenzy.top

[S30] C：头文件保护
来源：http://ltl.vqdsnc.cn

#ifndef X_H
来源：http://trc.sufxvd.cn

#define X_H
来源：http://ukn.ydzc1.top

#endif
来源：http://pqt.yuanzhike.top

[S31] C++：Hello World
来源：http://tdj.shuidangran.top

#include <iostream>
来源：http://zmh.zhoulong.xyz

int main() { std::cout << "Hello\n"; }
来源：http://bco.ehwqpu.com

[S32] C++：字符串
来源：http://eie.jyoumei.cn

std::string s = "hi";  s += "!";
来源：http://cps.kuanghao11.cn

[S33] C++：vector 增删
来源：http://cay.yj20258.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rdd.aizwys.cn

[S34] C++：遍历 vector
来源：http://lbg.shzxlz.cn

for (auto &x : v) { std::cout << x; }
来源：http://vtv.xylfe.cn

[S35] C++：map
来源：http://tjm.shuidangran.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vlr.xuetiantiany.cn

[S36] C++：unordered_map
来源：http://ele.cqqwz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hqr.hnxiangtu.top

[S37] C++：set
来源：http://nla.snrcjt.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jef.aizwys.cn

[S38] C++：排序
来源：http://zjw.jinghuilouyu.cn

std::sort(v.begin(), v.end());
来源：http://bdz.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://vum.jyoumei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bip.gogol.net.cn

[S40] C++：查找元素
来源：http://ltn.ppjwa.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ykc.52xcode.cn

[S41] C++：类与构造函数
来源：http://jbc.yuanzhike.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vwk.shanyushiyangtech.top

[S42] C++：继承与虚函数
来源：http://spr.xuanzx.com

class B : public Base { public: void f() override {} };
来源：http://ocg.chenlongwang.top

[S43] C++：智能指针
来源：http://hyu.guannengcc.top

auto p = std::make_unique<int>(5);
来源：http://ref.jinqigufen.top

[S44] C++：引用传参
来源：http://vuy.zhengqikj.top

void inc(int &x) { ++x; }
来源：http://hxx.bbcook.cn

[S45] C++：lambda
来源：http://owj.shanyushiyangtech.top

auto add = [](int a, int b) { return a + b; };
来源：http://lgh.bbcook.cn

[S46] C++：函数模板
来源：http://vgl.snrcjt.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ege.chenzaomai.com

[S47] C++：结构化绑定遍历
来源：http://prp.yfazqb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hna.xziqi.cn

[S48] C++：逐行读文件
来源：http://pmq.pengpengdd.cyou

std::ifstream in("a.txt");  std::string line;
来源：http://iih.ydjk.org.cn

while (std::getline(in, line)) { }
来源：http://hin.xinyue.icu

[S49] C++：写文件
来源：http://ucm.zhengqikj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vqc.yvedp.cn

[S50] C++：格式化数字
来源：http://mjt.fengsongda.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kvw.shangyingyoupin.top

[S51] C++：显式类型转换
来源：http://wfd.chenjidiqi.icu

static_cast<double>(a) / b
来源：http://qsf.pengpengdd.cyou

[S52] C++：const 与 noexcept
来源：http://srx.shanyushiyangkeji.top


<!-- 参考信息 -->