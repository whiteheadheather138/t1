代发 wailian999

[Q86] 读取 JSON 字段
来源：http://ghk.gzhubu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://chl.daria6918.cn

[Q87] JSON 字段做条件
来源：http://myc.xinyue.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sjq.yuanzhike.top

[Q88] 行转列（条件聚合）
来源：http://xfa.bbcook.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://igw.zhaomingkeji.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uch.yonumen.top

[Q89] 判断表是否存在
来源：http://ajv.yuanzhike.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ubr.9152youxi.cn

[Q90] 生成序号列
来源：http://kbb.hammf.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xlr.hfpthk.cn

================================================================================
来源：http://naw.shuidangran.top

R. Bash 专题
来源：http://pes.uphjek.com

================================================================================
来源：http://ubb.ctjpmb.com

[R01] shebang 与严格模式
来源：http://bca.meibo888.top

#!/usr/bin/env bash
来源：http://jxc.sjlbkw.cn

set -euo pipefail
来源：http://ffv.cdnleiting.top

[R02] 变量赋值与使用
来源：http://yfy.bbcook.cn

name="Tom"; echo "$name"
来源：http://ogf.chenjidiqi.icu

[R03] 只读变量
来源：http://ort.wangdashe.top

readonly PI=3.14
来源：http://bnw.sweek.top

[R04] 位置参数
来源：http://oly.fehbvm.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zfh.cqqwz.cn

[R05] 参数默认值
来源：http://kck.fehbvm.com

name="${1:-default}"
来源：http://gvq.snrcjt.cn

[R06] 判断命令是否存在
来源：http://asq.hywenlv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eda.snrcjt.cn

[R07] if 判断文件
来源：http://aqt.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cdf.shzxlz.cn

[R08] 数值比较
来源：http://knt.hammf.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zxt.hfpthk.cn

[R09] 字符串比较
来源：http://sdk.jinqigufen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vwd.havefunace.top

[R10] 正则匹配
来源：http://uro.nwbrower.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lzh.sweek.top

[R11] case 多分支
来源：http://beh.zhixingplan.top

case "$1" in
来源：http://llv.bjfxy.top

start) echo "启动" ;;
来源：http://udd.ppjwa.cn

stop)  echo "停止" ;;
来源：http://mvh.dianchejie.cn

*)     echo "未知命令" ;;
来源：http://bln.shanyushiyangkeji.top

esac
来源：http://xkj.shuidangran.top

[R12] for 遍历文件
来源：http://jaq.ybcxt.top

for f in *.txt; do echo "$f"; done
来源：http://wlb.yfazqb.com

[R13] for 计数循环
来源：http://auo.nanxinkj.top

for i in {1..10}; do echo "$i"; done
来源：http://hbq.mhx1999.top

[R14] C 风格 for
来源：http://isp.xziqi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uef.zdqjudy.top

[R15] while 逐行读文件
来源：http://zqr.hysaishi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zcl.bjfxy.top

[R16] until 等待条件
来源：http://jwa.yuanzhike.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pnb.feifeiyinyue.top

[R17] 数组定义与取值
来源：http://zew.jyoumei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ecs.jinyuanbaomall.cn

[R18] 遍历数组
来源：http://fte.yanxiufei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lpc.zhongyouzk.top

[R19] 数组长度
来源：http://izy.redwolf501.top

echo "${#arr[@]}"
来源：http://dxc.uphjek.com

[R20] 关联数组（字典）
来源：http://xwg.hnqzz.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ylr.fktsv.cn

[R21] 字符串长度
来源：http://jxp.ppjwa.cn

echo "${#s}"
来源：http://uym.hywenlv.cn

[R22] 截取子串
来源：http://xix.andypj.xyz

echo "${s:0:5}"
来源：http://awf.tanke756.top

[R23] 字符串替换
来源：http://bhw.ybcxt.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hyg.cqqwz.cn

[R24] 大小写转换
来源：http://pea.pycfn.com

echo "${s^^}"; echo "${s,,}"
来源：http://ije.zdbjq.cn

[R25] 去后缀 / 去前缀
来源：http://rxg.jyoumei.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uka.hysaishi.cn

[R26] 命令替换
来源：http://cmv.fengsongda.top

now=$(date +%F); echo "$now"
来源：http://xce.zhixingplan.top

[R27] 算术展开
来源：http://zwz.jianghu66.top

echo $((1 + 2 * 3))
来源：http://how.yangfankeji.com

[R28] 浮点运算
来源：http://frx.fengsongda.top

echo "scale=2; 10/3" | bc
来源：http://tso.tianlin.xyz

[R29] 定义函数
来源：http://yzl.sweek.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eln.316326.xyz

[R30] 函数返回状态码
来源：http://oaw.gaohongyu789.top

f() { return 0; }; f || echo "失败了"
来源：http://dud.bbcook.cn

[R31] 局部变量
来源：http://ezn.nanxuanxn.top

f() { local x=1; echo "$x"; }
来源：http://hkj.zhengqikj.top

[R32] 参数个数校验
来源：http://pty.jiagoushi.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://toj.9152youxi.cn

[R33] 捕获错误并提示行号
来源：http://lit.zdqjudy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tgz.yfazqb.com

[R34] 退出时清理
来源：http://yyn.xziqi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://krb.zhoulong.xyz

[R35] 后台执行并等待
来源：http://uys.zycfv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dqc.zhengqikj.top

[R36] 并发执行多个任务
来源：http://xcy.xuanzx.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bih.xziqi.cn

[R37] 把输出赋给变量
来源：http://fms.shanyushiyangkeji.top

files=$(ls -1)
来源：http://gfz.zhongyouzk.top

[R38] 管道串联
来源：http://iik.chenlongwang.top

cat a.txt | grep -i error | wc -l
来源：http://xms.snrcjt.cn

[R39] 重定向标准输出与错误
来源：http://wtn.yj202588.top

cmd > out.log 2>&1
来源：http://jgp.hfpthk.cn

[R40] 追加写日志
来源：http://wwd.fktsv.cn

echo "log" >> out.log
来源：http://hdy.mhx1999.top

[R41] 丢弃输出
来源：http://szy.quarkkingdee.top

cmd >/dev/null 2>&1
来源：http://keh.sysykeji.top

[R42] 输入重定向
来源：http://wwh.zhiwuduotai.top

wc -l < a.txt
来源：http://squ.daxiang520.top

[R43] 按名字查找文件
来源：http://uot.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://pky.fktsv.cn

[R44] 按修改时间查找
来源：http://qom.xingfuxueyuan.xyz

find . -mtime -7 -type f
来源：http://qll.chenjidiqi.icu

[R45] 批量删除
来源：http://kyq.nwbrower.top

find . -name "*.tmp" -delete
来源：http://rum.gzhubu.top

[R46] 递归替换文件内容
来源：http://dhx.shangyingyoupin.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gnl.cdnleiting.top

[R47] sed 单行替换
来源：http://ksr.cdnleiting.top

sed -i 's/foo/bar/g' a.txt
来源：http://ncb.hfpthk.cn

[R48] awk 取指定列
来源：http://qpc.gogol.net.cn

awk '{print $1, $3}' a.txt
来源：http://ivr.hongshengwenyu.top

[R49] awk 带条件
来源：http://vmg.gaohongyu789.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dmp.fengsongda.top

[R50] awk 求和
来源：http://sxd.pengpengdd.cyou

awk '{s += $2} END {print s}' a.txt
来源：http://pul.cashguo.top

[R51] 排序去重取前几
来源：http://cuk.xuanzx.com

sort a.txt | uniq -c | sort -rn | head
来源：http://okt.ctjpmb.com

[R52] 统计行数
来源：http://uah.cheryme.top

wc -l a.txt
来源：http://zpc.hfpthk.cn

[R53] 查看文件头与实时尾
来源：http://qxm.zhaomingkeji.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uql.c1oappe.top

[R54] 比较两个文件
来源：http://sxx.sysykeji.top

diff a.txt b.txt
来源：http://pek.hnxiangtu.top

[R55] 压缩与解压
来源：http://tfn.dianchejie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sum.tarul.cn

[R56] 远程拷贝
来源：http://pxt.shzxlz.cn

scp file user@host:/path/
来源：http://krh.yonumen.top

[R57] 远程执行命令
来源：http://vmy.zycfv.cn

ssh user@host 'uptime'
来源：http://rqh.wangdashe.top

[R58] 下载文件
来源：http://rhw.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tqp.tarul.cn

[R59] 发 POST JSON
来源：http://nmo.wangshuangyany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oqx.cashguo.top

[R60] 只看 HTTP 状态码
来源：http://jge.hfpthk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oyt.yonumen.top

[R61] 磁盘占用
来源：http://pkh.bbcook.cn

df -h;  du -sh *
来源：http://ihy.zdbjq.cn

[R62] 找最占空间的文件
来源：http://mzk.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://zyr.gogol.net.cn

[R63] 内存与进程
来源：http://fqo.chenlongwang.top

free -h;  ps aux | grep nginx
来源：http://smo.tarul.cn

[R64] 结束进程
来源：http://omm.jinyuanbaomall.cn

kill -9 $(pgrep -f app.py)
来源：http://fpv.zhaomingkeji.xyz

[R65] 查看端口占用
来源：http://emp.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://heo.zdqjudy.top

[R66] 定时任务
来源：http://aov.zdbjq.cn

crontab -e;  crontab -l
来源：http://bmd.yuxming.cn

[R67] 生成随机十六进制串
来源：http://set.aizwys.cn

openssl rand -hex 16
来源：http://kwz.zhengqikj.top

[R68] 计算文件校验值
来源：http://kln.xinyue.icu

sha256sum a.txt;  md5sum a.txt
来源：http://cuj.tanke756.top

[R69] 生成随机密码
来源：http://uaq.xylfe.cn

head -c 16 /dev/urandom | base64
来源：http://evo.ydjk.org.cn

[R70] 时间戳与互转
来源：http://qhr.sufxvd.cn

date +%s;  date -d @1700000000
来源：http://het.hnqzz.top

[R71] 日期格式化
来源：http://mlu.xingfuxueyuan.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://orm.gogol.net.cn

[R72] 等待端口就绪
来源：http://ivq.guowangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://pur.0kj1m.cn

[R73] 分割大日志
来源：http://hce.cucudq.cn

split -l 1000 big.log part_
来源：http://scs.pycfn.com

[R74] 批量重命名
来源：http://cvq.yangfankeji.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xfe.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://uzc.zhengqikj.top

export PATH="$HOME/bin:$PATH"
来源：http://uhn.yfazqb.com

[R76] 使用临时文件
来源：http://rfj.hammf.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://btc.shanyushiyangtech.top

[R77] 读取用户输入
来源：http://iwa.9152youxi.cn

read -rp "请输入: " ans
来源：http://rpa.yj202588.top

[R78] 交互式菜单
来源：http://xpm.dashuyun.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bik.hnqzz.top

[R79] 解析命令行选项
来源：http://iem.hcnkem.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dva.tanke756.top

[R80] 查看脚本执行耗时
来源：http://lpd.yuxming.cn

time ./run.sh
来源：http://hqy.aizwys.cn

================================================================================
来源：http://hsa.mhx1999.top

S. C / C++ 专题
来源：http://cct.gogol.net.cn

================================================================================
来源：http://obi.aibaodan.cn

[S01] C：Hello World
来源：http://zho.jinqigfzy.top

#include <stdio.h>
来源：http://mcl.sxryk.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cax.fanxiaobao.xyz

[S02] C：变量与格式化输出
来源：http://yoe.jiagoushi.top

int a = 10; printf("%d\n", a);
来源：http://lkk.pycfn.com

[S03] C：读入整数
来源：http://wkz.ivvv.top

int x; scanf("%d", &x);
来源：http://pna.pengpengdd.cyou

[S04] C：字符串复制
来源：http://wnh.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ueu.kuanghao11.cn

[S05] C：字符串长度
来源：http://xux.shzxlz.cn

strlen(s)
来源：http://tid.xylfe.cn

[S06] C：字符串比较
来源：http://qea.9152youxi.cn

strcmp(a, b) == 0
来源：http://kds.hnxiangtu.top

[S07] C：数组遍历求和
来源：http://vod.dianchejie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lqx.hongshengwenyu.top

[S08] C：动态内存分配与释放
来源：http://hrs.yonumen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mgt.bjfxy.top

[S09] C：结构体定义与初始化
来源：http://dwb.smart0.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://syk.shuidangran.top

[S10] C：指针与解引用
来源：http://bvl.jlsjyb.cn

int *p = &a;  *p = 5;
来源：http://upl.ydjk.org.cn

[S11] C：逐行读文件
来源：http://jjr.yangfankeji.com

FILE *f = fopen("a.txt", "r");
来源：http://jvm.bbcook.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lws.shanyushiyangkeji.top

fclose(f);
来源：http://gec.wangdashe.top

[S12] C：写文件
来源：http://suv.aibaodan.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wvs.xinyue.icu

[S13] C：宏定义
来源：http://mod.gaohongyu789.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rsz.fzhhl.top

[S14] C：枚举
来源：http://xlq.zdbjq.cn

enum Color { RED, GREEN, BLUE };
来源：http://ocy.daria6918.cn

[S15] C：类型转换
来源：http://dfi.gaohongyu789.top

(double) a / b
来源：http://gic.aibaodan.cn

[S16] C：位操作置位
来源：http://juu.hnqzz.top

x |= (1 << 3);
来源：http://psp.epnwcf.com

[S17] C：安全拼接字符串
来源：http://abl.uphjek.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mit.yonumen.top

[S18] C：命令行参数
来源：http://nbc.ivvv.top

int main(int argc, char **argv)
来源：http://dxo.fengsongda.top

[S19] C：快速排序
来源：http://wmc.zhijiandao.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cdx.svipenyu.cn

[S20] C：二分查找
来源：http://lnn.zhixingplan.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://smb.yvedp.cn

[S21] C：字符类别判断
来源：http://fsu.ybcxt.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://quk.jqgufenzy.top

[S22] C：字符串转数字
来源：http://rpw.andypj.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://gxv.sxryk.cn

[S23] C：随机数
来源：http://urn.wangdashe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bnx.ppjwa.cn

[S24] C：获取本地时间
来源：http://efx.kuanghao11.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hfx.haohaochexian.top

[S25] C：内存拷贝
来源：http://kwg.shangyingyoupin.top

memcpy(dst, src, n);
来源：http://klz.c1oappe.top

[S26] C：内存清零
来源：http://jzq.xuanzx.com

memset(a, 0, sizeof a);
来源：http://zbv.meibo888.top

[S27] C：定义常量
来源：http://uqo.yongpay.top

const double PI = 3.14159;
来源：http://tlq.shangyingyoupin.top

[S28] C：静态变量
来源：http://cpz.dianchejie.cn

static int counter = 0;
来源：http://woy.52xcode.cn

[S29] C：变参函数
来源：http://xwh.chenjidiqi.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kbq.sufxvd.cn

[S30] C：头文件保护
来源：http://myy.jinyuanbaomall.cn

#ifndef X_H
来源：http://ela.chenlongwang.top

#define X_H
来源：http://cgy.fengsongda.top

#endif
来源：http://hch.cashguo.top

[S31] C++：Hello World
来源：http://ues.ybcxt.top

#include <iostream>
来源：http://uyj.xuanzx.com

int main() { std::cout << "Hello\n"; }
来源：http://idt.pengpengdd.cyou

[S32] C++：字符串
来源：http://zim.bbcook.cn

std::string s = "hi";  s += "!";
来源：http://uob.havefunace.top

[S33] C++：vector 增删
来源：http://kob.sxryk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://twr.chenlongwang.top

[S34] C++：遍历 vector
来源：http://slc.epnwcf.com

for (auto &x : v) { std::cout << x; }
来源：http://beb.quarkkingdee.top

[S35] C++：map
来源：http://txx.ppjwa.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ehi.hcnkem.com

[S36] C++：unordered_map
来源：http://fzs.gzhubu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bhz.yongpay.top

[S37] C++：set
来源：http://abe.0kj1m.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qkl.feifeiyinyue.top

[S38] C++：排序
来源：http://szo.shangyingyoupin.top

std::sort(v.begin(), v.end());
来源：http://xbs.zhijiandao.cn

[S39] C++：自定义比较器排序
来源：http://onc.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mwo.ctjpmb.com

[S40] C++：查找元素
来源：http://hwb.vehdjk.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sht.jiagoushi.top

[S41] C++：类与构造函数
来源：http://rtn.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dyh.jinyuanbaomall.cn

[S42] C++：继承与虚函数
来源：http://nft.chenlongwang.top

class B : public Base { public: void f() override {} };
来源：http://gfg.jinghuilouyu.cn

[S43] C++：智能指针
来源：http://ace.ivvv.top

auto p = std::make_unique<int>(5);
来源：http://zgk.vqdsnc.cn

[S44] C++：引用传参
来源：http://rei.yvedp.cn

void inc(int &x) { ++x; }
来源：http://bwq.xziqi.cn

[S45] C++：lambda
来源：http://mwi.epnwcf.com

auto add = [](int a, int b) { return a + b; };
来源：http://svk.cqqwz.cn

[S46] C++：函数模板
来源：http://umd.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ggh.zhixingplan.top

[S47] C++：结构化绑定遍历
来源：http://mnx.cdnleiting.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kib.316326.xyz

[S48] C++：逐行读文件
来源：http://gjk.bjfxy.top

std::ifstream in("a.txt");  std::string line;
来源：http://vgl.jqgfzy.top

while (std::getline(in, line)) { }
来源：http://uay.jlsjyb.cn

[S49] C++：写文件
来源：http://cwk.iojbl.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://byx.zhijiandao.cn

[S50] C++：格式化数字
来源：http://lxi.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lqx.ctjpmb.com

[S51] C++：显式类型转换
来源：http://bei.yonumen.top

static_cast<double>(a) / b
来源：http://ggr.gaohongyu789.top

[S52] C++：const 与 noexcept
来源：http://ihw.yfazqb.com

int size() const noexcept { return n_; }
来源：http://lyd.birdmap.top

[S53] C++：移动语义
来源：http://nym.zhongyouzk.top

std::vector<int> w = std::move(v);
来源：http://znu.xinyue.icu

[S54] C++：异常处理
来源：http://ynq.xuetiantiany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ami.jinqigfzy.top

[S55] C++：结构化绑定
来源：http://jqh.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://aff.tianlin.xyz

[S56] C++：optional
来源：http://pww.bjfxy.top


<!-- 参考信息 -->