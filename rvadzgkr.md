代发 wailian999

[Q82] 字符长度与字节长度
来源：http://wch.shanyushiyangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yjz.daria6918.cn

[Q83] 大小写转换
来源：http://vcw.ydjk.org.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ioh.0kj1m.cn

[Q84] 去除首尾空格
来源：http://ync.jinyuanbaomall.cn

SELECT TRIM(name) FROM users;
来源：http://yta.9152youxi.cn

[Q85] 数值取整
来源：http://oar.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hxi.xylfe.cn

[Q86] 读取 JSON 字段
来源：http://tqy.yfazqb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yep.meibo888.top

[Q87] JSON 字段做条件
来源：http://hpl.9152youxi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hit.nanxinkj.top

[Q88] 行转列（条件聚合）
来源：http://eww.xuanzx.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://twx.chenzaomai.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sju.nanxinkj.top

[Q89] 判断表是否存在
来源：http://gnu.vqdsnc.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hve.jinyuanbaomall.cn

[Q90] 生成序号列
来源：http://ipa.cheryme.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jzt.quarkkingdee.top

================================================================================
来源：http://hds.sxryk.cn

R. Bash 专题
来源：http://zbk.jqgufenzy.top

================================================================================
来源：http://hrx.aibaodan.cn

[R01] shebang 与严格模式
来源：http://gwu.yuanzhike.top

#!/usr/bin/env bash
来源：http://bhe.jqgfzy.top

set -euo pipefail
来源：http://dcq.ehwqpu.com

[R02] 变量赋值与使用
来源：http://ajf.hnxiangtu.top

name="Tom"; echo "$name"
来源：http://avn.yuanzhike.top

[R03] 只读变量
来源：http://gbn.316326.xyz

readonly PI=3.14
来源：http://fxp.xylfe.cn

[R04] 位置参数
来源：http://ayd.yongpay.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mko.xuetiantiany.cn

[R05] 参数默认值
来源：http://coi.haohaochexian.top

name="${1:-default}"
来源：http://jut.sjlbkw.cn

[R06] 判断命令是否存在
来源：http://zrr.cheryme.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pwe.redwolf501.top

[R07] if 判断文件
来源：http://ntp.nanxinkj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uva.gaohongyu789.top

[R08] 数值比较
来源：http://ppr.ydzc1.top

if (( a > b )); then echo "a 更大"; fi
来源：http://uqw.fanxiaobao.xyz

[R09] 字符串比较
来源：http://buh.chenjidiqi.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lqm.ppjwa.cn

[R10] 正则匹配
来源：http://bdm.sweek.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dsk.jinghuilouyu.cn

[R11] case 多分支
来源：http://wvn.pycfn.com

case "$1" in
来源：http://ktf.yfazqb.com

start) echo "启动" ;;
来源：http://iaf.daria6918.cn

stop)  echo "停止" ;;
来源：http://kgp.gzhubu.top

*)     echo "未知命令" ;;
来源：http://oby.nanxinkj.top

esac
来源：http://tyr.tian-w.cn

[R12] for 遍历文件
来源：http://fyo.hfpthk.cn

for f in *.txt; do echo "$f"; done
来源：http://ohu.fengsongda.top

[R13] for 计数循环
来源：http://cvb.jiagoushi.top

for i in {1..10}; do echo "$i"; done
来源：http://neq.ivvv.top

[R14] C 风格 for
来源：http://pzx.sjlbkw.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://spf.yangfankeji.com

[R15] while 逐行读文件
来源：http://uor.xziqi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zib.bjfxy.top

[R16] until 等待条件
来源：http://qlo.yongpay.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zqa.shzxlz.cn

[R17] 数组定义与取值
来源：http://orz.svipenyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mmm.yj20258.top

[R18] 遍历数组
来源：http://rfl.xylfe.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kcp.cucudq.cn

[R19] 数组长度
来源：http://fqg.chenjidiqi.icu

echo "${#arr[@]}"
来源：http://tcp.yongpay.top

[R20] 关联数组（字典）
来源：http://yot.tian-w.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jnv.nanxuanxn.top

[R21] 字符串长度
来源：http://qxz.jinghuilouyu.cn

echo "${#s}"
来源：http://qws.cucudq.cn

[R22] 截取子串
来源：http://vwc.zdqjudy.top

echo "${s:0:5}"
来源：http://hwk.ivvv.top

[R23] 字符串替换
来源：http://lby.yangfankeji.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ahp.gotoacloud.top

[R24] 大小写转换
来源：http://ixo.tianlin.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://dpi.fzhhl.top

[R25] 去后缀 / 去前缀
来源：http://arz.gogol.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lav.zhixingplan.top

[R26] 命令替换
来源：http://xcz.sxryk.cn

now=$(date +%F); echo "$now"
来源：http://ryg.zhiwuduotai.top

[R27] 算术展开
来源：http://rzp.jiagoushi.top

echo $((1 + 2 * 3))
来源：http://lql.sufxvd.cn

[R28] 浮点运算
来源：http://yuq.xingfuxueyuan.xyz

echo "scale=2; 10/3" | bc
来源：http://dbz.yj20258888.top

[R29] 定义函数
来源：http://wht.zhaomingkeji.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kif.yj20258.top

[R30] 函数返回状态码
来源：http://znq.gotoacloud.top

f() { return 0; }; f || echo "失败了"
来源：http://cir.yj20258888.top

[R31] 局部变量
来源：http://epo.yfazqb.com

f() { local x=1; echo "$x"; }
来源：http://ljc.52xcode.cn

[R32] 参数个数校验
来源：http://ykj.zhixingplan.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qik.hnqzz.top

[R33] 捕获错误并提示行号
来源：http://gvu.dashuyun.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kvg.gaohongyu789.top

[R34] 退出时清理
来源：http://yvl.zycfv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dzn.cheryme.top

[R35] 后台执行并等待
来源：http://wgv.yj202588.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dsk.nwbrower.top

[R36] 并发执行多个任务
来源：http://vbp.epnwcf.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gyw.daria6918.cn

[R37] 把输出赋给变量
来源：http://dbg.ppjwa.cn

files=$(ls -1)
来源：http://zal.nanxinkj.top

[R38] 管道串联
来源：http://hxq.zhiwuduotai.top

cat a.txt | grep -i error | wc -l
来源：http://omx.xylfe.cn

[R39] 重定向标准输出与错误
来源：http://tqs.sysykeji.top

cmd > out.log 2>&1
来源：http://yap.chenjidiqi.icu

[R40] 追加写日志
来源：http://btw.c1oappe.top

echo "log" >> out.log
来源：http://igh.shanyushiyangkeji.top

[R41] 丢弃输出
来源：http://tuo.mhx1999.top

cmd >/dev/null 2>&1
来源：http://ocu.cashguo.top

[R42] 输入重定向
来源：http://qnt.quarkkingdee.top

wc -l < a.txt
来源：http://nhq.yj202588.top

[R43] 按名字查找文件
来源：http://cbe.fktsv.cn

find . -name "*.log" -type f
来源：http://tld.shzxlz.cn

[R44] 按修改时间查找
来源：http://irq.chenzaomai.com

find . -mtime -7 -type f
来源：http://xol.cashguo.top

[R45] 批量删除
来源：http://vfr.daria6918.cn

find . -name "*.tmp" -delete
来源：http://zbq.zhiwuduotai.top

[R46] 递归替换文件内容
来源：http://kdv.hongshengwenyu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fqg.c1oappe.top

[R47] sed 单行替换
来源：http://fat.cdnleiting.top

sed -i 's/foo/bar/g' a.txt
来源：http://oea.aizwys.cn

[R48] awk 取指定列
来源：http://xgb.tianlin.xyz

awk '{print $1, $3}' a.txt
来源：http://qjz.jqgfzy.top

[R49] awk 带条件
来源：http://zqb.hysaishi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zxr.fzhhl.top

[R50] awk 求和
来源：http://jgh.havefunace.top

awk '{s += $2} END {print s}' a.txt
来源：http://nzh.gotoacloud.top

[R51] 排序去重取前几
来源：http://kqw.ybcxt.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hcb.nanxinkj.top

[R52] 统计行数
来源：http://cwi.guannengcc.top

wc -l a.txt
来源：http://gow.hnxiangtu.top

[R53] 查看文件头与实时尾
来源：http://qhw.zdbjq.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qof.quarkkingdee.top

[R54] 比较两个文件
来源：http://lrt.hesvh.cn

diff a.txt b.txt
来源：http://pbf.dianchejie.cn

[R55] 压缩与解压
来源：http://nib.shangyingyoupin.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tzz.zhixingplan.top

[R56] 远程拷贝
来源：http://bwc.xingfuxueyuan.xyz

scp file user@host:/path/
来源：http://rsa.fzhhl.top

[R57] 远程执行命令
来源：http://ypv.shuidangran.top

ssh user@host 'uptime'
来源：http://pun.daxiang520.top

[R58] 下载文件
来源：http://fub.feifeiyinyue.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tdk.fengsongda.top

[R59] 发 POST JSON
来源：http://dfw.jyoumei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jye.yj202588.top

[R60] 只看 HTTP 状态码
来源：http://ryn.hongshengwenyu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ozc.pycfn.com

[R61] 磁盘占用
来源：http://xjd.hfpthk.cn

df -h;  du -sh *
来源：http://xqr.hfpthk.cn

[R62] 找最占空间的文件
来源：http://pvh.jianghu66.top

du -ah . | sort -rh | head -10
来源：http://fyp.pycfn.com

[R63] 内存与进程
来源：http://jty.aibaodan.cn

free -h;  ps aux | grep nginx
来源：http://nuh.haohaochexian.top

[R64] 结束进程
来源：http://rap.chenzaomai.com

kill -9 $(pgrep -f app.py)
来源：http://udl.gotoacloud.top

[R65] 查看端口占用
来源：http://xhr.hnxiangtu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wyd.yanxiufei.cn

[R66] 定时任务
来源：http://rik.tian-w.cn

crontab -e;  crontab -l
来源：http://ddc.meibo888.top

[R67] 生成随机十六进制串
来源：http://eak.shanyushiyangkeji.top

openssl rand -hex 16
来源：http://mjv.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://yuk.epnwcf.com

sha256sum a.txt;  md5sum a.txt
来源：http://toq.hfpthk.cn

[R69] 生成随机密码
来源：http://ffl.tianlin.xyz

head -c 16 /dev/urandom | base64
来源：http://uum.cheryme.top

[R70] 时间戳与互转
来源：http://szq.xinyue.icu

date +%s;  date -d @1700000000
来源：http://gqa.bjfxy.top

[R71] 日期格式化
来源：http://pmm.hammf.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wgl.chenzaomai.com

[R72] 等待端口就绪
来源：http://pps.vehdjk.com

until nc -z localhost 3306; do sleep 1; done
来源：http://bjs.jinghuilouyu.cn

[R73] 分割大日志
来源：http://gct.vqdsnc.cn

split -l 1000 big.log part_
来源：http://ngs.ydzc1.top

[R74] 批量重命名
来源：http://skn.smart0.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vnn.yanxiufei.cn

[R75] 导出环境变量
来源：http://bnp.pycfn.com

export PATH="$HOME/bin:$PATH"
来源：http://yne.zhoulong.xyz

[R76] 使用临时文件
来源：http://eoe.hammf.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pnj.hongshengwenyu.top

[R77] 读取用户输入
来源：http://vdn.yfazqb.com

read -rp "请输入: " ans
来源：http://oxm.redwolf501.top

[R78] 交互式菜单
来源：http://hgc.fzhhl.top

select opt in a b c; do echo "$opt"; break; done
来源：http://veh.aizwys.cn

[R79] 解析命令行选项
来源：http://wdy.0kj1m.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hvb.cucudq.cn

[R80] 查看脚本执行耗时
来源：http://zxw.vehdjk.com

time ./run.sh
来源：http://yyr.yj20258.top

================================================================================
来源：http://dgm.316326.xyz

S. C / C++ 专题
来源：http://noq.yuxming.cn

================================================================================
来源：http://zjc.nwbrower.top

[S01] C：Hello World
来源：http://gmd.bjfxy.top

#include <stdio.h>
来源：http://xsv.ybcxt.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ppd.zhixingplan.top

[S02] C：变量与格式化输出
来源：http://tnk.quarkkingdee.top

int a = 10; printf("%d\n", a);
来源：http://kpi.tianlin.xyz

[S03] C：读入整数
来源：http://fal.svipenyu.cn

int x; scanf("%d", &x);
来源：http://nnb.tianlin.xyz

[S04] C：字符串复制
来源：http://hkh.zhijiandao.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jlo.sweek.top

[S05] C：字符串长度
来源：http://qqg.xinyue.icu

strlen(s)
来源：http://pgd.cashguo.top

[S06] C：字符串比较
来源：http://fle.xinyue.icu

strcmp(a, b) == 0
来源：http://utk.guowangkeji.top

[S07] C：数组遍历求和
来源：http://uyo.jqgfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rus.hnxiangtu.top

[S08] C：动态内存分配与释放
来源：http://jpv.dashuyun.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yge.bjfxy.top

[S09] C：结构体定义与初始化
来源：http://fyu.cucudq.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://brs.yuxming.cn

[S10] C：指针与解引用
来源：http://gkn.xziqi.cn

int *p = &a;  *p = 5;
来源：http://ynu.yueranfly.top

[S11] C：逐行读文件
来源：http://oxz.zhijiandao.cn

FILE *f = fopen("a.txt", "r");
来源：http://gam.hongshengwenyu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jxz.shanyushiyangkeji.top

fclose(f);
来源：http://yqz.yj20258888.top

[S12] C：写文件
来源：http://guw.hywenlv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vvc.zhoulong.xyz

[S13] C：宏定义
来源：http://ruk.0kj1m.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uxy.cashguo.top

[S14] C：枚举
来源：http://asu.zhijiandao.cn

enum Color { RED, GREEN, BLUE };
来源：http://aye.ivvv.top

[S15] C：类型转换
来源：http://zhc.hnxiangtu.top

(double) a / b
来源：http://xto.c1oappe.top

[S16] C：位操作置位
来源：http://pbt.yonumen.top

x |= (1 << 3);
来源：http://jlq.ehwqpu.com

[S17] C：安全拼接字符串
来源：http://gcc.fktsv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://prr.shanyushiyangkeji.top

[S18] C：命令行参数
来源：http://wld.tanke756.top

int main(int argc, char **argv)
来源：http://rdd.svipenyu.cn

[S19] C：快速排序
来源：http://jfh.xingfuxueyuan.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://sjg.gotoacloud.top

[S20] C：二分查找
来源：http://eld.zdbjq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://trz.dashuyun.cn

[S21] C：字符类别判断
来源：http://ouh.yueranfly.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ipk.jinyuanbaomall.cn

[S22] C：字符串转数字
来源：http://rjy.bjfxy.top

atoi("42");  strtod("3.14", NULL);
来源：http://rgh.iojbl.cn

[S23] C：随机数
来源：http://nhf.zycfv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tiw.zhaomingkeji.xyz

[S24] C：获取本地时间
来源：http://jse.bjfxy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kfl.yfazqb.com

[S25] C：内存拷贝
来源：http://qdk.tanke756.top

memcpy(dst, src, n);
来源：http://ndx.dianchejie.cn

[S26] C：内存清零
来源：http://mvd.dashuyun.cn

memset(a, 0, sizeof a);
来源：http://ttf.yonumen.top

[S27] C：定义常量
来源：http://xgi.zhaomingkeji.xyz

const double PI = 3.14159;
来源：http://yph.gotoacloud.top

[S28] C：静态变量
来源：http://vou.dashuyun.cn

static int counter = 0;
来源：http://vll.yj20258888.top

[S29] C：变参函数
来源：http://awe.bjfxy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nqi.nwbrower.top

[S30] C：头文件保护
来源：http://ijy.gogol.net.cn

#ifndef X_H
来源：http://sqi.xuanzx.com

#define X_H
来源：http://wle.iojbl.cn

#endif
来源：http://tch.pengpengdd.cyou

[S31] C++：Hello World
来源：http://ydp.zdbjq.cn

#include <iostream>
来源：http://tzv.9152youxi.cn

int main() { std::cout << "Hello\n"; }
来源：http://tkk.hongshengwenyu.top

[S32] C++：字符串
来源：http://cjh.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://xpb.dianchejie.cn

[S33] C++：vector 增删
来源：http://brg.shzxlz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tdu.andypj.xyz

[S34] C++：遍历 vector
来源：http://zfc.chenjidiqi.icu

for (auto &x : v) { std::cout << x; }
来源：http://oot.redwolf501.top

[S35] C++：map
来源：http://jji.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ozd.guowangkeji.top

[S36] C++：unordered_map
来源：http://krj.yangfankeji.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fwy.jinyuanbaomall.cn

[S37] C++：set
来源：http://hvf.hcnkem.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dtv.xuetiantiany.cn

[S38] C++：排序
来源：http://dfd.andypj.xyz

std::sort(v.begin(), v.end());
来源：http://egc.havefunace.top

[S39] C++：自定义比较器排序
来源：http://eum.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ohz.zhiwuduotai.top

[S40] C++：查找元素
来源：http://wmz.yonumen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ocy.yanxiufei.cn

[S41] C++：类与构造函数
来源：http://bbg.zhongyouzk.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tdg.hesvh.cn

[S42] C++：继承与虚函数
来源：http://beo.cdnleiting.top

class B : public Base { public: void f() override {} };
来源：http://sua.cheryme.top

[S43] C++：智能指针
来源：http://xvp.nwbrower.top

auto p = std::make_unique<int>(5);
来源：http://xok.hesvh.cn

[S44] C++：引用传参
来源：http://tnr.ydzc1.top

void inc(int &x) { ++x; }
来源：http://rud.ydzc1.top

[S45] C++：lambda
来源：http://yjc.hesvh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://avr.jianghu66.top

[S46] C++：函数模板
来源：http://aat.zdbjq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ckh.kuanghao11.cn

[S47] C++：结构化绑定遍历
来源：http://hun.xuetiantiany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ynq.jqgfzy.top

[S48] C++：逐行读文件
来源：http://oqu.nanxinkj.top

std::ifstream in("a.txt");  std::string line;
来源：http://ktc.ybcxt.top

while (std::getline(in, line)) { }
来源：http://yha.tarul.cn

[S49] C++：写文件
来源：http://efo.yongpay.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zzz.hywenlv.cn

[S50] C++：格式化数字
来源：http://ggr.sysykeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qhy.pengpengdd.cyou

[S51] C++：显式类型转换
来源：http://dhc.wangshuangyany.cn

static_cast<double>(a) / b
来源：http://ewi.vehdjk.com

[S52] C++：const 与 noexcept
来源：http://our.daxiang520.top


<!-- 参考信息 -->