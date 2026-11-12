代发 wailian999

[Q84] 去除首尾空格
来源：http://qdh.nanxinkj.top

SELECT TRIM(name) FROM users;
来源：http://cxp.zhaomingkeji.xyz

[Q85] 数值取整
来源：http://wzt.aizwys.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rne.redwolf501.top

[Q86] 读取 JSON 字段
来源：http://flv.fehbvm.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zgp.yj20258.top

[Q87] JSON 字段做条件
来源：http://myt.9152youxi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tbw.dashuyun.cn

[Q88] 行转列（条件聚合）
来源：http://qpn.yuxming.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oxs.xinyue.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pzb.gaohongyu789.top

[Q89] 判断表是否存在
来源：http://wsp.zhoulong.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ieb.yangfankeji.com

[Q90] 生成序号列
来源：http://ypi.redwolf501.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qug.fehbvm.com

================================================================================
来源：http://mip.chenlongwang.top

R. Bash 专题
来源：http://pml.zhixingplan.top

================================================================================
来源：http://obo.jqgfzy.top

[R01] shebang 与严格模式
来源：http://myp.c1oappe.top

#!/usr/bin/env bash
来源：http://zrf.meibo888.top

set -euo pipefail
来源：http://ghs.gogol.net.cn

[R02] 变量赋值与使用
来源：http://jrz.shuidangran.top

name="Tom"; echo "$name"
来源：http://llx.jinqigfzy.top

[R03] 只读变量
来源：http://znp.guowangkeji.top

readonly PI=3.14
来源：http://ihm.vqdsnc.cn

[R04] 位置参数
来源：http://bft.havefunace.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qmd.ehwqpu.com

[R05] 参数默认值
来源：http://quu.hywenlv.cn

name="${1:-default}"
来源：http://lwm.jiagoushi.top

[R06] 判断命令是否存在
来源：http://wcs.cashguo.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://afi.zycfv.cn

[R07] if 判断文件
来源：http://qje.jlsjyb.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dvv.dashuyun.cn

[R08] 数值比较
来源：http://gck.gogol.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://osb.gogol.net.cn

[R09] 字符串比较
来源：http://lyo.sxryk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qur.gotoacloud.top

[R10] 正则匹配
来源：http://qvc.jinqigufen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uye.cqqwz.cn

[R11] case 多分支
来源：http://jqd.zhoulong.xyz

case "$1" in
来源：http://rii.ywan-chungtsiang.top

start) echo "启动" ;;
来源：http://mxt.iojbl.cn

stop)  echo "停止" ;;
来源：http://jnz.feifeiyinyue.top

*)     echo "未知命令" ;;
来源：http://cqg.guowangkeji.top

esac
来源：http://crq.jinqigfzy.top

[R12] for 遍历文件
来源：http://bow.52xcode.cn

for f in *.txt; do echo "$f"; done
来源：http://gsd.dashuyun.cn

[R13] for 计数循环
来源：http://rap.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://zml.zdqjudy.top

[R14] C 风格 for
来源：http://wdd.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qap.yj20258888.top

[R15] while 逐行读文件
来源：http://dto.yvedp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rax.gzhubu.top

[R16] until 等待条件
来源：http://bjt.zhengqikj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pqp.xylfe.cn

[R17] 数组定义与取值
来源：http://qqx.tanke756.top

arr=(a b c); echo "${arr[0]}"
来源：http://xpz.jiagoushi.top

[R18] 遍历数组
来源：http://dux.jinyuanbaomall.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zov.zdqjudy.top

[R19] 数组长度
来源：http://mrn.birdmap.top

echo "${#arr[@]}"
来源：http://nwn.tian-w.cn

[R20] 关联数组（字典）
来源：http://dld.yuanzhike.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bti.ctjpmb.com

[R21] 字符串长度
来源：http://rgd.andypj.xyz

echo "${#s}"
来源：http://kuj.cqqwz.cn

[R22] 截取子串
来源：http://nmq.daria6918.cn

echo "${s:0:5}"
来源：http://eck.ydjk.org.cn

[R23] 字符串替换
来源：http://khq.snrcjt.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://udy.quarkkingdee.top

[R24] 大小写转换
来源：http://yxq.xuetiantiany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nvj.tianlin.xyz

[R25] 去后缀 / 去前缀
来源：http://cpu.zhongyouzk.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://cmn.shuidangran.top

[R26] 命令替换
来源：http://yoq.yj20258888.top

now=$(date +%F); echo "$now"
来源：http://mct.svipenyu.cn

[R27] 算术展开
来源：http://kbu.vqdsnc.cn

echo $((1 + 2 * 3))
来源：http://ijm.shangyingyoupin.top

[R28] 浮点运算
来源：http://dxo.yj20258.top

echo "scale=2; 10/3" | bc
来源：http://wsk.ydjk.org.cn

[R29] 定义函数
来源：http://avu.gogol.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://unq.hnxiangtu.top

[R30] 函数返回状态码
来源：http://cdz.ydjk.org.cn

f() { return 0; }; f || echo "失败了"
来源：http://fta.bbcook.cn

[R31] 局部变量
来源：http://bqk.zhijiandao.cn

f() { local x=1; echo "$x"; }
来源：http://neh.zhoulong.xyz

[R32] 参数个数校验
来源：http://cji.zhijiandao.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kai.hfpthk.cn

[R33] 捕获错误并提示行号
来源：http://vth.sysykeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ohx.jiagoushi.top

[R34] 退出时清理
来源：http://frm.sxryk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ldl.sysykeji.top

[R35] 后台执行并等待
来源：http://iom.uphjek.com

sleep 5 & pid=$!; wait "$pid"
来源：http://egt.jianghu66.top

[R36] 并发执行多个任务
来源：http://nhc.316326.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vtn.aibaodan.cn

[R37] 把输出赋给变量
来源：http://hox.gotoacloud.top

files=$(ls -1)
来源：http://lcb.sysykeji.top

[R38] 管道串联
来源：http://vgx.pengpengdd.cyou

cat a.txt | grep -i error | wc -l
来源：http://hkz.tian-w.cn

[R39] 重定向标准输出与错误
来源：http://vvh.dianchejie.cn

cmd > out.log 2>&1
来源：http://pqd.pycfn.com

[R40] 追加写日志
来源：http://orp.guowangkeji.top

echo "log" >> out.log
来源：http://buy.daria6918.cn

[R41] 丢弃输出
来源：http://vya.sjlbkw.cn

cmd >/dev/null 2>&1
来源：http://fpw.jinqigfzy.top

[R42] 输入重定向
来源：http://hna.316326.xyz

wc -l < a.txt
来源：http://bur.bbcook.cn

[R43] 按名字查找文件
来源：http://xll.nanxuanxn.top

find . -name "*.log" -type f
来源：http://tfb.gogol.net.cn

[R44] 按修改时间查找
来源：http://yul.bjfxy.top

find . -mtime -7 -type f
来源：http://amu.gotoacloud.top

[R45] 批量删除
来源：http://krb.dashuyun.cn

find . -name "*.tmp" -delete
来源：http://zqr.zdbjq.cn

[R46] 递归替换文件内容
来源：http://kvx.shangyingyoupin.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sma.xziqi.cn

[R47] sed 单行替换
来源：http://glr.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://xfw.ehwqpu.com

[R48] awk 取指定列
来源：http://clq.bjfxy.top

awk '{print $1, $3}' a.txt
来源：http://ten.zhijiandao.cn

[R49] awk 带条件
来源：http://vnw.jianghu66.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bel.cashguo.top

[R50] awk 求和
来源：http://mfk.guowangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://pyg.vehdjk.com

[R51] 排序去重取前几
来源：http://dag.daxiang520.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ztm.chenjidiqi.icu

[R52] 统计行数
来源：http://kto.birdmap.top

wc -l a.txt
来源：http://oac.bbcook.cn

[R53] 查看文件头与实时尾
来源：http://mto.zdqjudy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kma.xuanzx.com

[R54] 比较两个文件
来源：http://ndz.jinghuilouyu.cn

diff a.txt b.txt
来源：http://cjh.sufxvd.cn

[R55] 压缩与解压
来源：http://gyi.jiagoushi.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tyz.nanxuanxn.top

[R56] 远程拷贝
来源：http://zug.smart0.xyz

scp file user@host:/path/
来源：http://uyw.zhiwuduotai.top

[R57] 远程执行命令
来源：http://ppe.shangyingyoupin.top

ssh user@host 'uptime'
来源：http://zxg.hammf.cn

[R58] 下载文件
来源：http://hiy.dashuyun.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xnl.meibo888.top

[R59] 发 POST JSON
来源：http://usp.daria6918.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jyq.zhijiandao.cn

[R60] 只看 HTTP 状态码
来源：http://dwi.hesvh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bre.haohaochexian.top

[R61] 磁盘占用
来源：http://pqy.wangshuangyany.cn

df -h;  du -sh *
来源：http://dif.guannengcc.top

[R62] 找最占空间的文件
来源：http://ebj.nwbrower.top

du -ah . | sort -rh | head -10
来源：http://mav.hnqzz.top

[R63] 内存与进程
来源：http://rhj.jinyuanbaomall.cn

free -h;  ps aux | grep nginx
来源：http://uej.yueranfly.top

[R64] 结束进程
来源：http://hbj.ybcxt.top

kill -9 $(pgrep -f app.py)
来源：http://rzf.xuanzx.com

[R65] 查看端口占用
来源：http://zaa.dashuyun.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ygg.yueranfly.top

[R66] 定时任务
来源：http://muw.52xcode.cn

crontab -e;  crontab -l
来源：http://ajr.mhx1999.top

[R67] 生成随机十六进制串
来源：http://jmc.cdnleiting.top

openssl rand -hex 16
来源：http://tmo.nanxinkj.top

[R68] 计算文件校验值
来源：http://tro.nwbrower.top

sha256sum a.txt;  md5sum a.txt
来源：http://qic.zdbjq.cn

[R69] 生成随机密码
来源：http://vuu.nwbrower.top

head -c 16 /dev/urandom | base64
来源：http://tpj.havefunace.top

[R70] 时间戳与互转
来源：http://rxn.zhixingplan.top

date +%s;  date -d @1700000000
来源：http://quf.chenzaomai.com

[R71] 日期格式化
来源：http://vmw.bjfxy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://buw.yueranfly.top

[R72] 等待端口就绪
来源：http://lvr.gotoacloud.top

until nc -z localhost 3306; do sleep 1; done
来源：http://owa.wangdashe.top

[R73] 分割大日志
来源：http://qxs.tarul.cn

split -l 1000 big.log part_
来源：http://zuj.cdnleiting.top

[R74] 批量重命名
来源：http://ynt.daria6918.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xcn.haohaochexian.top

[R75] 导出环境变量
来源：http://wcz.hnqzz.top

export PATH="$HOME/bin:$PATH"
来源：http://jci.zhongyouzk.top

[R76] 使用临时文件
来源：http://nst.jinyuanbaomall.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sew.redwolf501.top

[R77] 读取用户输入
来源：http://gca.hnqzz.top

read -rp "请输入: " ans
来源：http://ocj.tianlin.xyz

[R78] 交互式菜单
来源：http://wxr.tanke756.top

select opt in a b c; do echo "$opt"; break; done
来源：http://lsz.cucudq.cn

[R79] 解析命令行选项
来源：http://dam.uphjek.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eap.zhaomingkeji.xyz

[R80] 查看脚本执行耗时
来源：http://sbs.ydjk.org.cn

time ./run.sh
来源：http://tds.vqdsnc.cn

================================================================================
来源：http://obi.xuanzx.com

S. C / C++ 专题
来源：http://bai.gotoacloud.top

================================================================================
来源：http://hqd.xuanzx.com

[S01] C：Hello World
来源：http://bed.gzhubu.top

#include <stdio.h>
来源：http://xon.zhiwuduotai.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jrr.birdmap.top

[S02] C：变量与格式化输出
来源：http://ocy.ywan-chungtsiang.top

int a = 10; printf("%d\n", a);
来源：http://xxh.sjlbkw.cn

[S03] C：读入整数
来源：http://kkl.ywan-chungtsiang.top

int x; scanf("%d", &x);
来源：http://lpv.jqgufenzy.top

[S04] C：字符串复制
来源：http://wbt.shangyingyoupin.top

char dst[32]; strcpy(dst, "hi");
来源：http://uix.zhengqikj.top

[S05] C：字符串长度
来源：http://tvw.nanxinkj.top

strlen(s)
来源：http://sca.aizwys.cn

[S06] C：字符串比较
来源：http://qcy.xziqi.cn

strcmp(a, b) == 0
来源：http://hhr.yfazqb.com

[S07] C：数组遍历求和
来源：http://uwy.hywenlv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://awc.zhiwuduotai.top

[S08] C：动态内存分配与释放
来源：http://kqw.jianghu66.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fnb.zhijiandao.cn

[S09] C：结构体定义与初始化
来源：http://twe.ppjwa.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ded.ivvv.top

[S10] C：指针与解引用
来源：http://pqe.daria6918.cn

int *p = &a;  *p = 5;
来源：http://mis.fanxiaobao.xyz

[S11] C：逐行读文件
来源：http://mwi.aizwys.cn

FILE *f = fopen("a.txt", "r");
来源：http://ybc.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wni.gzhubu.top

fclose(f);
来源：http://nnp.yj202588.top

[S12] C：写文件
来源：http://bkr.zycfv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ixg.shanyushiyangkeji.top

[S13] C：宏定义
来源：http://jpr.pengpengdd.cyou

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jdn.andypj.xyz

[S14] C：枚举
来源：http://nxz.aibaodan.cn

enum Color { RED, GREEN, BLUE };
来源：http://kwn.pycfn.com

[S15] C：类型转换
来源：http://apa.tarul.cn

(double) a / b
来源：http://hmh.meibo888.top

[S16] C：位操作置位
来源：http://icc.quarkkingdee.top

x |= (1 << 3);
来源：http://jct.ywan-chungtsiang.top

[S17] C：安全拼接字符串
来源：http://wwc.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yjh.cqqwz.cn

[S18] C：命令行参数
来源：http://cis.iojbl.cn

int main(int argc, char **argv)
来源：http://bpr.fktsv.cn

[S19] C：快速排序
来源：http://jar.fanxiaobao.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://zrt.guannengcc.top

[S20] C：二分查找
来源：http://iwy.daria6918.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gjk.ydzc1.top

[S21] C：字符类别判断
来源：http://vlg.jiagoushi.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://htv.iojbl.cn

[S22] C：字符串转数字
来源：http://bht.0kj1m.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tff.xylfe.cn

[S23] C：随机数
来源：http://cxf.jinqigfzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vkp.gogol.net.cn

[S24] C：获取本地时间
来源：http://jju.cashguo.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yac.zhijiandao.cn

[S25] C：内存拷贝
来源：http://szy.aibaodan.cn

memcpy(dst, src, n);
来源：http://ncb.ehwqpu.com

[S26] C：内存清零
来源：http://cwn.xuanzx.com

memset(a, 0, sizeof a);
来源：http://hod.yongpay.top

[S27] C：定义常量
来源：http://wsw.snrcjt.cn

const double PI = 3.14159;
来源：http://hvw.hammf.cn

[S28] C：静态变量
来源：http://jhz.gogol.net.cn

static int counter = 0;
来源：http://qam.zdqjudy.top

[S29] C：变参函数
来源：http://dgc.fehbvm.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uff.zdbjq.cn

[S30] C：头文件保护
来源：http://dke.yongpay.top

#ifndef X_H
来源：http://dtu.jinghuilouyu.cn

#define X_H
来源：http://cgn.fzhhl.top

#endif
来源：http://yot.feifeiyinyue.top

[S31] C++：Hello World
来源：http://zeh.cdnleiting.top

#include <iostream>
来源：http://sfs.wangdashe.top

int main() { std::cout << "Hello\n"; }
来源：http://fjm.sysykeji.top

[S32] C++：字符串
来源：http://kyi.xinyue.icu

std::string s = "hi";  s += "!";
来源：http://hqq.smart0.xyz

[S33] C++：vector 增删
来源：http://guu.jlsjyb.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dtw.sufxvd.cn

[S34] C++：遍历 vector
来源：http://zcb.sxryk.cn

for (auto &x : v) { std::cout << x; }
来源：http://pci.yangfankeji.com

[S35] C++：map
来源：http://oqq.cdnleiting.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rlj.hnqzz.top

[S36] C++：unordered_map
来源：http://was.yj20258888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ppz.shanyushiyangkeji.top

[S37] C++：set
来源：http://mwv.zhaomingkeji.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bki.xylfe.cn

[S38] C++：排序
来源：http://whh.hysaishi.cn

std::sort(v.begin(), v.end());
来源：http://kyq.c1oappe.top

[S39] C++：自定义比较器排序
来源：http://jlj.xziqi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cos.fzhhl.top

[S40] C++：查找元素
来源：http://wot.xylfe.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ern.jinghuilouyu.cn

[S41] C++：类与构造函数
来源：http://xbe.316326.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vbx.wangdashe.top

[S42] C++：继承与虚函数
来源：http://sky.yueranfly.top

class B : public Base { public: void f() override {} };
来源：http://hhy.ybcxt.top

[S43] C++：智能指针
来源：http://zcp.cucudq.cn

auto p = std::make_unique<int>(5);
来源：http://xfr.hongshengwenyu.top

[S44] C++：引用传参
来源：http://tje.birdmap.top

void inc(int &x) { ++x; }
来源：http://eof.sxryk.cn

[S45] C++：lambda
来源：http://fyb.shuidangran.top

auto add = [](int a, int b) { return a + b; };
来源：http://orm.xziqi.cn

[S46] C++：函数模板
来源：http://ftu.vehdjk.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fav.zhixingplan.top

[S47] C++：结构化绑定遍历
来源：http://fcl.iojbl.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hbk.feifeiyinyue.top

[S48] C++：逐行读文件
来源：http://yzc.vqdsnc.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qpi.316326.xyz

while (std::getline(in, line)) { }
来源：http://ipt.fanxiaobao.xyz

[S49] C++：写文件
来源：http://fvc.hesvh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jjc.xuanzx.com

[S50] C++：格式化数字
来源：http://svx.jyoumei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://crf.zhongyouzk.top

[S51] C++：显式类型转换
来源：http://gvj.yanxiufei.cn

static_cast<double>(a) / b
来源：http://wkj.zdbjq.cn

[S52] C++：const 与 noexcept
来源：http://eek.chenjidiqi.icu

int size() const noexcept { return n_; }
来源：http://ptf.dashuyun.cn

[S53] C++：移动语义
来源：http://tbj.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://fjf.epnwcf.com

[S54] C++：异常处理
来源：http://ino.316326.xyz


<!-- 参考信息 -->