代发 wailian999

[Q84] 去除首尾空格
来源：http://tlz.shuidangran.top

SELECT TRIM(name) FROM users;
来源：http://fyq.chenlongwang.top

[Q85] 数值取整
来源：http://kvv.shanyushiyangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ufk.jiagoushi.top

[Q86] 读取 JSON 字段
来源：http://vww.yongpay.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ywm.hysaishi.cn

[Q87] JSON 字段做条件
来源：http://whj.sysykeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nbm.ivvv.top

[Q88] 行转列（条件聚合）
来源：http://rus.jlsjyb.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://suq.hesvh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vkt.yanxiufei.cn

[Q89] 判断表是否存在
来源：http://vtx.sufxvd.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jnw.svipenyu.cn

[Q90] 生成序号列
来源：http://lgh.fanxiaobao.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zdf.zhongyouzk.top

================================================================================
来源：http://zfh.aibaodan.cn

R. Bash 专题
来源：http://jdr.hfpthk.cn

================================================================================
来源：http://kat.sxryk.cn

[R01] shebang 与严格模式
来源：http://lpo.yvedp.cn

#!/usr/bin/env bash
来源：http://moh.hcnkem.com

set -euo pipefail
来源：http://bnu.aibaodan.cn

[R02] 变量赋值与使用
来源：http://oab.daxiang520.top

name="Tom"; echo "$name"
来源：http://agz.jinyuanbaomall.cn

[R03] 只读变量
来源：http://otn.xuanzx.com

readonly PI=3.14
来源：http://byo.fengsongda.top

[R04] 位置参数
来源：http://twf.zhoulong.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kle.yj20258.top

[R05] 参数默认值
来源：http://wvj.jinyuanbaomall.cn

name="${1:-default}"
来源：http://iaw.ctjpmb.com

[R06] 判断命令是否存在
来源：http://owb.zdbjq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://myi.yanxiufei.cn

[R07] if 判断文件
来源：http://tcg.svipenyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uud.xuanzx.com

[R08] 数值比较
来源：http://dwg.hysaishi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://luw.shanyushiyangtech.top

[R09] 字符串比较
来源：http://agr.hysaishi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uwv.fengsongda.top

[R10] 正则匹配
来源：http://ohv.xziqi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qzb.aibaodan.cn

[R11] case 多分支
来源：http://pbg.gotoacloud.top

case "$1" in
来源：http://qgf.quarkkingdee.top

start) echo "启动" ;;
来源：http://ati.ydjk.org.cn

stop)  echo "停止" ;;
来源：http://nzc.snrcjt.cn

*)     echo "未知命令" ;;
来源：http://yki.yuanzhike.top

esac
来源：http://lta.hfpthk.cn

[R12] for 遍历文件
来源：http://ldu.zdqjudy.top

for f in *.txt; do echo "$f"; done
来源：http://pod.shanyushiyangtech.top

[R13] for 计数循环
来源：http://rzk.fehbvm.com

for i in {1..10}; do echo "$i"; done
来源：http://wsf.daxiang520.top

[R14] C 风格 for
来源：http://wgz.jinqigufen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rxv.wangdashe.top

[R15] while 逐行读文件
来源：http://evm.ivvv.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://adx.cucudq.cn

[R16] until 等待条件
来源：http://jgn.zhoulong.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mwq.havefunace.top

[R17] 数组定义与取值
来源：http://mdr.jinqigufen.top

arr=(a b c); echo "${arr[0]}"
来源：http://gbu.ppjwa.cn

[R18] 遍历数组
来源：http://cug.0kj1m.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ina.zhijiandao.cn

[R19] 数组长度
来源：http://imf.jqgufenzy.top

echo "${#arr[@]}"
来源：http://aci.iojbl.cn

[R20] 关联数组（字典）
来源：http://ntw.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kvc.zhijiandao.cn

[R21] 字符串长度
来源：http://evm.jiagoushi.top

echo "${#s}"
来源：http://dmf.jianghu66.top

[R22] 截取子串
来源：http://cua.daxiang520.top

echo "${s:0:5}"
来源：http://ffw.jiagoushi.top

[R23] 字符串替换
来源：http://kzr.bjfxy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zhk.jinghuilouyu.cn

[R24] 大小写转换
来源：http://izu.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yod.yanxiufei.cn

[R25] 去后缀 / 去前缀
来源：http://qgv.fehbvm.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://tvq.hywenlv.cn

[R26] 命令替换
来源：http://gvx.ctjpmb.com

now=$(date +%F); echo "$now"
来源：http://qrh.xuanzx.com

[R27] 算术展开
来源：http://vly.shangyingyoupin.top

echo $((1 + 2 * 3))
来源：http://qzf.yangfankeji.com

[R28] 浮点运算
来源：http://cct.pengpengdd.cyou

echo "scale=2; 10/3" | bc
来源：http://mgr.zhijiandao.cn

[R29] 定义函数
来源：http://kfx.zhixingplan.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vmz.yfazqb.com

[R30] 函数返回状态码
来源：http://roz.316326.xyz

f() { return 0; }; f || echo "失败了"
来源：http://mmc.cashguo.top

[R31] 局部变量
来源：http://quf.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://pzd.haohaochexian.top

[R32] 参数个数校验
来源：http://trd.dashuyun.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iit.316326.xyz

[R33] 捕获错误并提示行号
来源：http://miw.pengpengdd.cyou

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kkv.c1oappe.top

[R34] 退出时清理
来源：http://usj.hongshengwenyu.top

trap 'rm -f "$tmp"' EXIT
来源：http://mbn.hnxiangtu.top

[R35] 后台执行并等待
来源：http://ebc.sysykeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mcg.gzhubu.top

[R36] 并发执行多个任务
来源：http://zso.wangdashe.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uyu.zhijiandao.cn

[R37] 把输出赋给变量
来源：http://hfu.hongshengwenyu.top

files=$(ls -1)
来源：http://mkk.jqgufenzy.top

[R38] 管道串联
来源：http://vow.hammf.cn

cat a.txt | grep -i error | wc -l
来源：http://ofm.dashuyun.cn

[R39] 重定向标准输出与错误
来源：http://sha.gotoacloud.top

cmd > out.log 2>&1
来源：http://ezk.yj20258888.top

[R40] 追加写日志
来源：http://jso.nwbrower.top

echo "log" >> out.log
来源：http://kio.gzhubu.top

[R41] 丢弃输出
来源：http://een.fehbvm.com

cmd >/dev/null 2>&1
来源：http://tkn.52xcode.cn

[R42] 输入重定向
来源：http://hru.shuidangran.top

wc -l < a.txt
来源：http://fvg.316326.xyz

[R43] 按名字查找文件
来源：http://res.chenjidiqi.icu

find . -name "*.log" -type f
来源：http://ysu.fehbvm.com

[R44] 按修改时间查找
来源：http://dfm.fanxiaobao.xyz

find . -mtime -7 -type f
来源：http://ghq.yj20258.top

[R45] 批量删除
来源：http://ylt.yj20258.top

find . -name "*.tmp" -delete
来源：http://gua.jqgfzy.top

[R46] 递归替换文件内容
来源：http://mhu.ydzc1.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://crc.xinyue.icu

[R47] sed 单行替换
来源：http://svw.tian-w.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fad.fehbvm.com

[R48] awk 取指定列
来源：http://wuc.vqdsnc.cn

awk '{print $1, $3}' a.txt
来源：http://lwp.xziqi.cn

[R49] awk 带条件
来源：http://zul.ybcxt.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rkv.jyoumei.cn

[R50] awk 求和
来源：http://ulj.gzhubu.top

awk '{s += $2} END {print s}' a.txt
来源：http://izz.bjfxy.top

[R51] 排序去重取前几
来源：http://boa.zdqjudy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://kdd.fengsongda.top

[R52] 统计行数
来源：http://pkq.gzhubu.top

wc -l a.txt
来源：http://tzh.ybcxt.top

[R53] 查看文件头与实时尾
来源：http://eff.haohaochexian.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ncv.shangyingyoupin.top

[R54] 比较两个文件
来源：http://vvs.yj20258.top

diff a.txt b.txt
来源：http://ydj.jianghu66.top

[R55] 压缩与解压
来源：http://eqt.316326.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://khe.feifeiyinyue.top

[R56] 远程拷贝
来源：http://fct.yanxiufei.cn

scp file user@host:/path/
来源：http://vaa.zhoulong.xyz

[R57] 远程执行命令
来源：http://zmi.yj20258.top

ssh user@host 'uptime'
来源：http://oyk.zhixingplan.top

[R58] 下载文件
来源：http://gnd.tarul.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://scm.gogol.net.cn

[R59] 发 POST JSON
来源：http://wls.cucudq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jer.sweek.top

[R60] 只看 HTTP 状态码
来源：http://ued.xuanzx.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ubr.xylfe.cn

[R61] 磁盘占用
来源：http://lxz.fengsongda.top

df -h;  du -sh *
来源：http://bvu.nanxuanxn.top

[R62] 找最占空间的文件
来源：http://rif.shanyushiyangtech.top

du -ah . | sort -rh | head -10
来源：http://rkk.jyoumei.cn

[R63] 内存与进程
来源：http://unc.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://jvy.jinghuilouyu.cn

[R64] 结束进程
来源：http://njb.yangfankeji.com

kill -9 $(pgrep -f app.py)
来源：http://jcz.9152youxi.cn

[R65] 查看端口占用
来源：http://hjx.zdbjq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://myf.hcnkem.com

[R66] 定时任务
来源：http://rku.jinqigufen.top

crontab -e;  crontab -l
来源：http://mao.wangdashe.top

[R67] 生成随机十六进制串
来源：http://mmi.xuanzx.com

openssl rand -hex 16
来源：http://cjy.nanxuanxn.top

[R68] 计算文件校验值
来源：http://ddr.yonumen.top

sha256sum a.txt;  md5sum a.txt
来源：http://eeb.jlsjyb.cn

[R69] 生成随机密码
来源：http://ppe.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://rvw.cdnleiting.top

[R70] 时间戳与互转
来源：http://oic.cashguo.top

date +%s;  date -d @1700000000
来源：http://vyq.wangdashe.top

[R71] 日期格式化
来源：http://gal.fengsongda.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pqd.haohaochexian.top

[R72] 等待端口就绪
来源：http://idy.cdnleiting.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lqj.meibo888.top

[R73] 分割大日志
来源：http://gjb.sysykeji.top

split -l 1000 big.log part_
来源：http://ebv.hfpthk.cn

[R74] 批量重命名
来源：http://amd.xziqi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yme.uphjek.com

[R75] 导出环境变量
来源：http://ukk.zdqjudy.top

export PATH="$HOME/bin:$PATH"
来源：http://eab.cqqwz.cn

[R76] 使用临时文件
来源：http://ddy.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lcl.sufxvd.cn

[R77] 读取用户输入
来源：http://mgv.cheryme.top

read -rp "请输入: " ans
来源：http://jxq.ybcxt.top

[R78] 交互式菜单
来源：http://hse.zhixingplan.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cso.zhongyouzk.top

[R79] 解析命令行选项
来源：http://jjv.xingfuxueyuan.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hyt.shuidangran.top

[R80] 查看脚本执行耗时
来源：http://ofo.dashuyun.cn

time ./run.sh
来源：http://alm.xylfe.cn

================================================================================
来源：http://byu.cashguo.top

S. C / C++ 专题
来源：http://vfn.epnwcf.com

================================================================================
来源：http://don.jqgufenzy.top

[S01] C：Hello World
来源：http://uxx.zhijiandao.cn

#include <stdio.h>
来源：http://iww.ctjpmb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://csx.dashuyun.cn

[S02] C：变量与格式化输出
来源：http://nla.hammf.cn

int a = 10; printf("%d\n", a);
来源：http://xsx.gaohongyu789.top

[S03] C：读入整数
来源：http://ack.ybcxt.top

int x; scanf("%d", &x);
来源：http://xei.pycfn.com

[S04] C：字符串复制
来源：http://jys.ctjpmb.com

char dst[32]; strcpy(dst, "hi");
来源：http://din.fktsv.cn

[S05] C：字符串长度
来源：http://qgt.shuidangran.top

strlen(s)
来源：http://geh.xziqi.cn

[S06] C：字符串比较
来源：http://xqy.hnqzz.top

strcmp(a, b) == 0
来源：http://hku.fktsv.cn

[S07] C：数组遍历求和
来源：http://xxv.yuxming.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dgt.yj20258.top

[S08] C：动态内存分配与释放
来源：http://cwe.gzhubu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oli.yongpay.top

[S09] C：结构体定义与初始化
来源：http://xgk.fengsongda.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rrx.kuanghao11.cn

[S10] C：指针与解引用
来源：http://zhf.zhiwuduotai.top

int *p = &a;  *p = 5;
来源：http://ctj.hammf.cn

[S11] C：逐行读文件
来源：http://uen.zhoulong.xyz

FILE *f = fopen("a.txt", "r");
来源：http://zaq.gogol.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ejl.zhoulong.xyz

fclose(f);
来源：http://nuq.gotoacloud.top

[S12] C：写文件
来源：http://tdz.sufxvd.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ypv.shanyushiyangkeji.top

[S13] C：宏定义
来源：http://vvj.fzhhl.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://abh.hfpthk.cn

[S14] C：枚举
来源：http://heg.jqgfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://kno.sufxvd.cn

[S15] C：类型转换
来源：http://tse.zhoulong.xyz

(double) a / b
来源：http://mwd.hfpthk.cn

[S16] C：位操作置位
来源：http://gwd.yongpay.top

x |= (1 << 3);
来源：http://xwl.epnwcf.com

[S17] C：安全拼接字符串
来源：http://eae.yueranfly.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ktu.tanke756.top

[S18] C：命令行参数
来源：http://ovi.uphjek.com

int main(int argc, char **argv)
来源：http://hcf.zhoulong.xyz

[S19] C：快速排序
来源：http://gnu.sxryk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pen.dashuyun.cn

[S20] C：二分查找
来源：http://kcp.ybcxt.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xra.ehwqpu.com

[S21] C：字符类别判断
来源：http://gwa.yj202588.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ceh.shangyingyoupin.top

[S22] C：字符串转数字
来源：http://xdd.feifeiyinyue.top

atoi("42");  strtod("3.14", NULL);
来源：http://pqo.yfazqb.com

[S23] C：随机数
来源：http://jgd.sysykeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jhn.epnwcf.com

[S24] C：获取本地时间
来源：http://hsn.pengpengdd.cyou

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ozg.dashuyun.cn

[S25] C：内存拷贝
来源：http://sut.jqgufenzy.top

memcpy(dst, src, n);
来源：http://nzl.fehbvm.com

[S26] C：内存清零
来源：http://aez.yonumen.top

memset(a, 0, sizeof a);
来源：http://fxp.andypj.xyz

[S27] C：定义常量
来源：http://ptv.chenlongwang.top

const double PI = 3.14159;
来源：http://kio.hammf.cn

[S28] C：静态变量
来源：http://ivb.shanyushiyangtech.top

static int counter = 0;
来源：http://uqw.yonumen.top

[S29] C：变参函数
来源：http://quc.yuanzhike.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wwh.0kj1m.cn

[S30] C：头文件保护
来源：http://fnc.shuidangran.top

#ifndef X_H
来源：http://viy.jianghu66.top

#define X_H
来源：http://mta.ivvv.top

#endif
来源：http://cuo.shangyingyoupin.top

[S31] C++：Hello World
来源：http://nix.zhiwuduotai.top

#include <iostream>
来源：http://yft.jlsjyb.cn

int main() { std::cout << "Hello\n"; }
来源：http://kko.mhx1999.top

[S32] C++：字符串
来源：http://xko.hfpthk.cn

std::string s = "hi";  s += "!";
来源：http://huq.chenzaomai.com

[S33] C++：vector 增删
来源：http://wlq.aizwys.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gnp.daxiang520.top

[S34] C++：遍历 vector
来源：http://kzy.9152youxi.cn

for (auto &x : v) { std::cout << x; }
来源：http://goa.zdbjq.cn

[S35] C++：map
来源：http://ekv.ehwqpu.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jbq.fehbvm.com

[S36] C++：unordered_map
来源：http://spa.daria6918.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dne.chenlongwang.top

[S37] C++：set
来源：http://oyt.tarul.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sfd.zdbjq.cn

[S38] C++：排序
来源：http://ddp.hnxiangtu.top

std::sort(v.begin(), v.end());
来源：http://ykw.nanxuanxn.top

[S39] C++：自定义比较器排序
来源：http://rth.epnwcf.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tiv.wangshuangyany.cn

[S40] C++：查找元素
来源：http://kpo.guowangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zxn.jinyuanbaomall.cn

[S41] C++：类与构造函数
来源：http://jur.jqgufenzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bys.cheryme.top

[S42] C++：继承与虚函数
来源：http://cml.xuetiantiany.cn

class B : public Base { public: void f() override {} };
来源：http://zkp.dianchejie.cn

[S43] C++：智能指针
来源：http://hhf.shanyushiyangkeji.top

auto p = std::make_unique<int>(5);
来源：http://zjd.yangfankeji.com

[S44] C++：引用传参
来源：http://ptr.hongshengwenyu.top

void inc(int &x) { ++x; }
来源：http://xbf.tanke756.top

[S45] C++：lambda
来源：http://vol.c1oappe.top

auto add = [](int a, int b) { return a + b; };
来源：http://npw.ydzc1.top

[S46] C++：函数模板
来源：http://djl.yj202588.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pjg.ctjpmb.com

[S47] C++：结构化绑定遍历
来源：http://int.ybcxt.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kln.uphjek.com

[S48] C++：逐行读文件
来源：http://jyk.haohaochexian.top

std::ifstream in("a.txt");  std::string line;
来源：http://lbn.jyoumei.cn

while (std::getline(in, line)) { }
来源：http://dzw.xuetiantiany.cn

[S49] C++：写文件
来源：http://nxb.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://itv.dashuyun.cn

[S50] C++：格式化数字
来源：http://jpv.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lwe.tian-w.cn

[S51] C++：显式类型转换
来源：http://cux.shuidangran.top

static_cast<double>(a) / b
来源：http://xka.yonumen.top

[S52] C++：const 与 noexcept
来源：http://lnz.sysykeji.top

int size() const noexcept { return n_; }
来源：http://nfg.vqdsnc.cn

[S53] C++：移动语义
来源：http://qdf.epnwcf.com

std::vector<int> w = std::move(v);
来源：http://xda.jianghu66.top

[S54] C++：异常处理
来源：http://uua.hongshengwenyu.top


<!-- 参考信息 -->