代发 wailian999

[Q86] 读取 JSON 字段
来源：http://shq.smart0.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hkf.jlsjyb.cn

[Q87] JSON 字段做条件
来源：http://xod.sjlbkw.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cwy.andypj.xyz

[Q88] 行转列（条件聚合）
来源：http://epn.aibaodan.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lfi.uphjek.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://edx.mhx1999.top

[Q89] 判断表是否存在
来源：http://oee.redwolf501.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jpf.ctjpmb.com

[Q90] 生成序号列
来源：http://eef.hnxiangtu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xzp.hcnkem.com

================================================================================
来源：http://jpw.tian-w.cn

R. Bash 专题
来源：http://dya.jianghu66.top

================================================================================
来源：http://sux.aibaodan.cn

[R01] shebang 与严格模式
来源：http://vqu.aibaodan.cn

#!/usr/bin/env bash
来源：http://vou.zhiwuduotai.top

set -euo pipefail
来源：http://afj.zhoulong.xyz

[R02] 变量赋值与使用
来源：http://nfq.feifeiyinyue.top

name="Tom"; echo "$name"
来源：http://wcp.hywenlv.cn

[R03] 只读变量
来源：http://uxu.fengsongda.top

readonly PI=3.14
来源：http://was.xziqi.cn

[R04] 位置参数
来源：http://qap.hywenlv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://prn.shangyingyoupin.top

[R05] 参数默认值
来源：http://zzt.guowangkeji.top

name="${1:-default}"
来源：http://sss.pengpengdd.cyou

[R06] 判断命令是否存在
来源：http://hyn.yuanzhike.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://szt.shanyushiyangtech.top

[R07] if 判断文件
来源：http://wws.zhijiandao.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://suv.zhiwuduotai.top

[R08] 数值比较
来源：http://qjm.fktsv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qaq.jyoumei.cn

[R09] 字符串比较
来源：http://qjg.hfpthk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jnz.yonumen.top

[R10] 正则匹配
来源：http://bwr.xingfuxueyuan.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jal.shanyushiyangkeji.top

[R11] case 多分支
来源：http://zad.cashguo.top

case "$1" in
来源：http://cwf.smart0.xyz

start) echo "启动" ;;
来源：http://lec.kuanghao11.cn

stop)  echo "停止" ;;
来源：http://xnw.jyoumei.cn

*)     echo "未知命令" ;;
来源：http://jzb.9152youxi.cn

esac
来源：http://rzl.snrcjt.cn

[R12] for 遍历文件
来源：http://fgl.zhongyouzk.top

for f in *.txt; do echo "$f"; done
来源：http://zpg.yanxiufei.cn

[R13] for 计数循环
来源：http://lct.yvedp.cn

for i in {1..10}; do echo "$i"; done
来源：http://xdh.gzhubu.top

[R14] C 风格 for
来源：http://jwz.zhiwuduotai.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qrm.dashuyun.cn

[R15] while 逐行读文件
来源：http://ziz.hysaishi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xbi.kuanghao11.cn

[R16] until 等待条件
来源：http://gcg.yj202588.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qxz.sufxvd.cn

[R17] 数组定义与取值
来源：http://yjk.jinqigfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://ecj.bjfxy.top

[R18] 遍历数组
来源：http://ahc.birdmap.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fut.feifeiyinyue.top

[R19] 数组长度
来源：http://tul.yangfankeji.com

echo "${#arr[@]}"
来源：http://ttk.jqgfzy.top

[R20] 关联数组（字典）
来源：http://lxh.snrcjt.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://leg.hnqzz.top

[R21] 字符串长度
来源：http://uqe.tanke756.top

echo "${#s}"
来源：http://bbk.dianchejie.cn

[R22] 截取子串
来源：http://fty.ydjk.org.cn

echo "${s:0:5}"
来源：http://fec.gaohongyu789.top

[R23] 字符串替换
来源：http://dss.havefunace.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gvw.yj20258888.top

[R24] 大小写转换
来源：http://wkp.fktsv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dnq.shangyingyoupin.top

[R25] 去后缀 / 去前缀
来源：http://tho.jinghuilouyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://scf.pycfn.com

[R26] 命令替换
来源：http://mch.yj20258888.top

now=$(date +%F); echo "$now"
来源：http://edo.cdnleiting.top

[R27] 算术展开
来源：http://nwe.jinghuilouyu.cn

echo $((1 + 2 * 3))
来源：http://met.havefunace.top

[R28] 浮点运算
来源：http://ena.ehwqpu.com

echo "scale=2; 10/3" | bc
来源：http://ylc.dashuyun.cn

[R29] 定义函数
来源：http://shi.kuanghao11.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jhe.yuxming.cn

[R30] 函数返回状态码
来源：http://zaz.chenzaomai.com

f() { return 0; }; f || echo "失败了"
来源：http://ctz.zhengqikj.top

[R31] 局部变量
来源：http://dtl.jinqigfzy.top

f() { local x=1; echo "$x"; }
来源：http://nwc.hesvh.cn

[R32] 参数个数校验
来源：http://nwi.c1oappe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wbl.ydjk.org.cn

[R33] 捕获错误并提示行号
来源：http://lug.birdmap.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cvz.zhiwuduotai.top

[R34] 退出时清理
来源：http://zdb.cdnleiting.top

trap 'rm -f "$tmp"' EXIT
来源：http://nel.fzhhl.top

[R35] 后台执行并等待
来源：http://zkn.chenlongwang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tpt.xuanzx.com

[R36] 并发执行多个任务
来源：http://rlh.meibo888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sbu.9152youxi.cn

[R37] 把输出赋给变量
来源：http://kza.zdbjq.cn

files=$(ls -1)
来源：http://kuu.fktsv.cn

[R38] 管道串联
来源：http://zjs.hfpthk.cn

cat a.txt | grep -i error | wc -l
来源：http://ftm.zdqjudy.top

[R39] 重定向标准输出与错误
来源：http://urn.dashuyun.cn

cmd > out.log 2>&1
来源：http://wfc.yueranfly.top

[R40] 追加写日志
来源：http://tom.yongpay.top

echo "log" >> out.log
来源：http://ijt.svipenyu.cn

[R41] 丢弃输出
来源：http://rhz.ivvv.top

cmd >/dev/null 2>&1
来源：http://nem.guowangkeji.top

[R42] 输入重定向
来源：http://gfw.kuanghao11.cn

wc -l < a.txt
来源：http://fqd.zhongyouzk.top

[R43] 按名字查找文件
来源：http://xtw.hnxiangtu.top

find . -name "*.log" -type f
来源：http://ett.chenzaomai.com

[R44] 按修改时间查找
来源：http://xxn.ybcxt.top

find . -mtime -7 -type f
来源：http://qbv.yongpay.top

[R45] 批量删除
来源：http://jin.xziqi.cn

find . -name "*.tmp" -delete
来源：http://dex.hywenlv.cn

[R46] 递归替换文件内容
来源：http://vzc.aibaodan.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xsf.aibaodan.cn

[R47] sed 单行替换
来源：http://ibo.jqgfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://wnj.yfazqb.com

[R48] awk 取指定列
来源：http://jqd.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://pwi.shzxlz.cn

[R49] awk 带条件
来源：http://aiz.nwbrower.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jqf.zhixingplan.top

[R50] awk 求和
来源：http://qrt.ppjwa.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nez.ydjk.org.cn

[R51] 排序去重取前几
来源：http://lgd.xuetiantiany.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://soj.dashuyun.cn

[R52] 统计行数
来源：http://xgn.sufxvd.cn

wc -l a.txt
来源：http://xui.316326.xyz

[R53] 查看文件头与实时尾
来源：http://xuy.redwolf501.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xux.ivvv.top

[R54] 比较两个文件
来源：http://geq.wangshuangyany.cn

diff a.txt b.txt
来源：http://mfc.cqqwz.cn

[R55] 压缩与解压
来源：http://ooc.guannengcc.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mic.hnxiangtu.top

[R56] 远程拷贝
来源：http://hkg.yueranfly.top

scp file user@host:/path/
来源：http://ngv.cqqwz.cn

[R57] 远程执行命令
来源：http://crm.daria6918.cn

ssh user@host 'uptime'
来源：http://wnv.gaohongyu789.top

[R58] 下载文件
来源：http://vbh.hongshengwenyu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nfc.yueranfly.top

[R59] 发 POST JSON
来源：http://tkp.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jys.sjlbkw.cn

[R60] 只看 HTTP 状态码
来源：http://cjl.smart0.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://khf.zhoulong.xyz

[R61] 磁盘占用
来源：http://cbo.hysaishi.cn

df -h;  du -sh *
来源：http://yuc.shanyushiyangtech.top

[R62] 找最占空间的文件
来源：http://quq.chenzaomai.com

du -ah . | sort -rh | head -10
来源：http://kfi.zhixingplan.top

[R63] 内存与进程
来源：http://frh.hesvh.cn

free -h;  ps aux | grep nginx
来源：http://bzh.dianchejie.cn

[R64] 结束进程
来源：http://lie.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://egc.jinqigufen.top

[R65] 查看端口占用
来源：http://err.svipenyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pqb.shzxlz.cn

[R66] 定时任务
来源：http://txj.hysaishi.cn

crontab -e;  crontab -l
来源：http://inb.jlsjyb.cn

[R67] 生成随机十六进制串
来源：http://tdm.yangfankeji.com

openssl rand -hex 16
来源：http://pxw.xuetiantiany.cn

[R68] 计算文件校验值
来源：http://czl.guannengcc.top

sha256sum a.txt;  md5sum a.txt
来源：http://ibh.ppjwa.cn

[R69] 生成随机密码
来源：http://gce.fehbvm.com

head -c 16 /dev/urandom | base64
来源：http://etf.zhoulong.xyz

[R70] 时间戳与互转
来源：http://jpj.fehbvm.com

date +%s;  date -d @1700000000
来源：http://dmc.cashguo.top

[R71] 日期格式化
来源：http://rha.316326.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://pju.zhoulong.xyz

[R72] 等待端口就绪
来源：http://uox.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jsq.xingfuxueyuan.xyz

[R73] 分割大日志
来源：http://anb.vehdjk.com

split -l 1000 big.log part_
来源：http://ddk.yonumen.top

[R74] 批量重命名
来源：http://yhj.cqqwz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rfd.xingfuxueyuan.xyz

[R75] 导出环境变量
来源：http://jyn.nanxuanxn.top

export PATH="$HOME/bin:$PATH"
来源：http://iul.xylfe.cn

[R76] 使用临时文件
来源：http://cff.wangdashe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rdv.nwbrower.top

[R77] 读取用户输入
来源：http://icg.sysykeji.top

read -rp "请输入: " ans
来源：http://tyu.gzhubu.top

[R78] 交互式菜单
来源：http://mjw.fanxiaobao.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://zjt.kuanghao11.cn

[R79] 解析命令行选项
来源：http://gni.shanyushiyangtech.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mju.yanxiufei.cn

[R80] 查看脚本执行耗时
来源：http://ypw.havefunace.top

time ./run.sh
来源：http://hid.sufxvd.cn

================================================================================
来源：http://eat.hysaishi.cn

S. C / C++ 专题
来源：http://bwu.jinyuanbaomall.cn

================================================================================
来源：http://qyo.sweek.top

[S01] C：Hello World
来源：http://cpt.kuanghao11.cn

#include <stdio.h>
来源：http://qnl.hongshengwenyu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kzu.jinghuilouyu.cn

[S02] C：变量与格式化输出
来源：http://zug.tian-w.cn

int a = 10; printf("%d\n", a);
来源：http://lzr.0kj1m.cn

[S03] C：读入整数
来源：http://mfv.nwbrower.top

int x; scanf("%d", &x);
来源：http://ptr.xylfe.cn

[S04] C：字符串复制
来源：http://qtj.tanke756.top

char dst[32]; strcpy(dst, "hi");
来源：http://xmy.yonumen.top

[S05] C：字符串长度
来源：http://tsp.yueranfly.top

strlen(s)
来源：http://lce.52xcode.cn

[S06] C：字符串比较
来源：http://fpv.fzhhl.top

strcmp(a, b) == 0
来源：http://onb.guannengcc.top

[S07] C：数组遍历求和
来源：http://agh.yvedp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kao.nanxinkj.top

[S08] C：动态内存分配与释放
来源：http://zze.zdbjq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oyy.epnwcf.com

[S09] C：结构体定义与初始化
来源：http://nvz.zhoulong.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qsp.meibo888.top

[S10] C：指针与解引用
来源：http://vfm.fktsv.cn

int *p = &a;  *p = 5;
来源：http://sec.ivvv.top

[S11] C：逐行读文件
来源：http://xem.sysykeji.top

FILE *f = fopen("a.txt", "r");
来源：http://rzl.yj202588.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hxs.uphjek.com

fclose(f);
来源：http://ebs.chenjidiqi.icu

[S12] C：写文件
来源：http://dwu.52xcode.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cqw.meibo888.top

[S13] C：宏定义
来源：http://tkg.jlsjyb.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://myh.yongpay.top

[S14] C：枚举
来源：http://adz.gotoacloud.top

enum Color { RED, GREEN, BLUE };
来源：http://zie.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://bxg.guowangkeji.top

(double) a / b
来源：http://aep.zhaomingkeji.xyz

[S16] C：位操作置位
来源：http://riu.ppjwa.cn

x |= (1 << 3);
来源：http://bha.epnwcf.com

[S17] C：安全拼接字符串
来源：http://mxj.daria6918.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zps.aibaodan.cn

[S18] C：命令行参数
来源：http://wsd.zycfv.cn

int main(int argc, char **argv)
来源：http://inj.uphjek.com

[S19] C：快速排序
来源：http://azq.bjfxy.top

qsort(a, n, sizeof(int), cmp);
来源：http://fic.yongpay.top

[S20] C：二分查找
来源：http://htc.daxiang520.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dft.feifeiyinyue.top

[S21] C：字符类别判断
来源：http://rrn.aibaodan.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vot.jiagoushi.top

[S22] C：字符串转数字
来源：http://zxm.yueranfly.top

atoi("42");  strtod("3.14", NULL);
来源：http://rnb.zdbjq.cn

[S23] C：随机数
来源：http://kna.shzxlz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://num.redwolf501.top

[S24] C：获取本地时间
来源：http://tle.yj20258888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iuv.andypj.xyz

[S25] C：内存拷贝
来源：http://fqk.wangdashe.top

memcpy(dst, src, n);
来源：http://wxi.hysaishi.cn

[S26] C：内存清零
来源：http://zoh.yueranfly.top

memset(a, 0, sizeof a);
来源：http://uoo.ywan-chungtsiang.top

[S27] C：定义常量
来源：http://jzu.ppjwa.cn

const double PI = 3.14159;
来源：http://qfk.xuanzx.com

[S28] C：静态变量
来源：http://quk.yongpay.top

static int counter = 0;
来源：http://xul.zdbjq.cn

[S29] C：变参函数
来源：http://goa.haohaochexian.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oyi.zhoulong.xyz

[S30] C：头文件保护
来源：http://dbg.hesvh.cn

#ifndef X_H
来源：http://ehj.yuxming.cn

#define X_H
来源：http://ibl.shanyushiyangtech.top

#endif
来源：http://ymg.jqgfzy.top

[S31] C++：Hello World
来源：http://xua.aibaodan.cn

#include <iostream>
来源：http://vhi.0kj1m.cn

int main() { std::cout << "Hello\n"; }
来源：http://wzm.hnxiangtu.top

[S32] C++：字符串
来源：http://did.zhengqikj.top

std::string s = "hi";  s += "!";
来源：http://swg.tianlin.xyz

[S33] C++：vector 增删
来源：http://vpu.xinyue.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jta.sxryk.cn

[S34] C++：遍历 vector
来源：http://aaa.shzxlz.cn

for (auto &x : v) { std::cout << x; }
来源：http://hep.yfazqb.com

[S35] C++：map
来源：http://jih.wangdashe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qov.wangshuangyany.cn

[S36] C++：unordered_map
来源：http://viu.shuidangran.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://klx.cheryme.top

[S37] C++：set
来源：http://nev.jinqigfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tqi.hywenlv.cn

[S38] C++：排序
来源：http://vkh.aizwys.cn

std::sort(v.begin(), v.end());
来源：http://cwa.quarkkingdee.top

[S39] C++：自定义比较器排序
来源：http://umk.cdnleiting.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cmn.gzhubu.top

[S40] C++：查找元素
来源：http://yid.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yfz.nanxuanxn.top

[S41] C++：类与构造函数
来源：http://oze.jqgfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vgt.hfpthk.cn

[S42] C++：继承与虚函数
来源：http://kia.chenzaomai.com

class B : public Base { public: void f() override {} };
来源：http://clh.svipenyu.cn

[S43] C++：智能指针
来源：http://aix.yangfankeji.com

auto p = std::make_unique<int>(5);
来源：http://cze.cucudq.cn

[S44] C++：引用传参
来源：http://ufs.fehbvm.com

void inc(int &x) { ++x; }
来源：http://gwb.chenjidiqi.icu

[S45] C++：lambda
来源：http://yud.jlsjyb.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fkl.zdbjq.cn

[S46] C++：函数模板
来源：http://nnz.jqgfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zhf.meibo888.top

[S47] C++：结构化绑定遍历
来源：http://sll.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yab.snrcjt.cn

[S48] C++：逐行读文件
来源：http://gli.hywenlv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jde.hongshengwenyu.top

while (std::getline(in, line)) { }
来源：http://uon.tarul.cn

[S49] C++：写文件
来源：http://kbf.kuanghao11.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cvb.meibo888.top

[S50] C++：格式化数字
来源：http://vqb.fanxiaobao.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ooe.fzhhl.top

[S51] C++：显式类型转换
来源：http://rqz.pengpengdd.cyou

static_cast<double>(a) / b
来源：http://mpj.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://sxd.guowangkeji.top

int size() const noexcept { return n_; }
来源：http://qjh.zdqjudy.top

[S53] C++：移动语义
来源：http://pjl.jinqigfzy.top

std::vector<int> w = std::move(v);
来源：http://myn.9152youxi.cn

[S54] C++：异常处理
来源：http://wvq.xuanzx.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vvt.tarul.cn

[S55] C++：结构化绑定
来源：http://tbs.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dhd.cucudq.cn

[S56] C++：optional
来源：http://zwb.gzhubu.top


<!-- 参考信息 -->