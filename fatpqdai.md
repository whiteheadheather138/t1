代发 wailian999

[Q80] 字符串截取
来源：http://mns.cucudq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qaf.ybcxt.top

[Q81] 字符串替换
来源：http://ehx.guowangkeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pjf.yj20258888.top

[Q82] 字符长度与字节长度
来源：http://ysl.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wfl.hywenlv.cn

[Q83] 大小写转换
来源：http://atr.chenzaomai.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://edy.quarkkingdee.top

[Q84] 去除首尾空格
来源：http://oxl.fanxiaobao.xyz

SELECT TRIM(name) FROM users;
来源：http://kxs.yuanzhike.top

[Q85] 数值取整
来源：http://fgh.cheryme.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gda.yuanzhike.top

[Q86] 读取 JSON 字段
来源：http://gxn.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wcp.jinyuanbaomall.cn

[Q87] JSON 字段做条件
来源：http://mid.nanxuanxn.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://afv.ctjpmb.com

[Q88] 行转列（条件聚合）
来源：http://yfk.zdqjudy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mya.dianchejie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pvr.nanxinkj.top

[Q89] 判断表是否存在
来源：http://nfp.ppjwa.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iya.guannengcc.top

[Q90] 生成序号列
来源：http://zbn.jinyuanbaomall.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ugm.gotoacloud.top

================================================================================
来源：http://tni.nanxinkj.top

R. Bash 专题
来源：http://mty.c1oappe.top

================================================================================
来源：http://jzb.andypj.xyz

[R01] shebang 与严格模式
来源：http://lvu.zhongyouzk.top

#!/usr/bin/env bash
来源：http://hzv.yonumen.top

set -euo pipefail
来源：http://jrr.aizwys.cn

[R02] 变量赋值与使用
来源：http://akc.hywenlv.cn

name="Tom"; echo "$name"
来源：http://ica.aibaodan.cn

[R03] 只读变量
来源：http://dff.yonumen.top

readonly PI=3.14
来源：http://bdm.feifeiyinyue.top

[R04] 位置参数
来源：http://iof.nanxuanxn.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qok.yuxming.cn

[R05] 参数默认值
来源：http://bwc.fehbvm.com

name="${1:-default}"
来源：http://vth.gotoacloud.top

[R06] 判断命令是否存在
来源：http://jdm.zdbjq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vzc.smart0.xyz

[R07] if 判断文件
来源：http://ncn.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://akg.nanxinkj.top

[R08] 数值比较
来源：http://sxc.uphjek.com

if (( a > b )); then echo "a 更大"; fi
来源：http://jls.jinyuanbaomall.cn

[R09] 字符串比较
来源：http://spp.hysaishi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wej.andypj.xyz

[R10] 正则匹配
来源：http://wwc.jiagoushi.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zih.mhx1999.top

[R11] case 多分支
来源：http://akc.ctjpmb.com

case "$1" in
来源：http://xwo.xylfe.cn

start) echo "启动" ;;
来源：http://hsw.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://iik.316326.xyz

*)     echo "未知命令" ;;
来源：http://sis.tian-w.cn

esac
来源：http://inu.hfpthk.cn

[R12] for 遍历文件
来源：http://zcp.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://cjm.cqqwz.cn

[R13] for 计数循环
来源：http://wqd.dashuyun.cn

for i in {1..10}; do echo "$i"; done
来源：http://nzr.sweek.top

[R14] C 风格 for
来源：http://rdo.fanxiaobao.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fvf.sxryk.cn

[R15] while 逐行读文件
来源：http://lwp.iojbl.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dvq.vqdsnc.cn

[R16] until 等待条件
来源：http://oqo.jinyuanbaomall.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rre.sxryk.cn

[R17] 数组定义与取值
来源：http://svk.ydjk.org.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ckn.ydzc1.top

[R18] 遍历数组
来源：http://xgx.wangdashe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://whj.ctjpmb.com

[R19] 数组长度
来源：http://agv.yuxming.cn

echo "${#arr[@]}"
来源：http://mli.iojbl.cn

[R20] 关联数组（字典）
来源：http://nug.hywenlv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oxi.chenlongwang.top

[R21] 字符串长度
来源：http://ays.havefunace.top

echo "${#s}"
来源：http://jdd.aibaodan.cn

[R22] 截取子串
来源：http://ezu.hysaishi.cn

echo "${s:0:5}"
来源：http://jcf.meibo888.top

[R23] 字符串替换
来源：http://aeg.9152youxi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gui.bjfxy.top

[R24] 大小写转换
来源：http://zub.zhongyouzk.top

echo "${s^^}"; echo "${s,,}"
来源：http://wsx.sufxvd.cn

[R25] 去后缀 / 去前缀
来源：http://gzx.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uxa.tanke756.top

[R26] 命令替换
来源：http://nxw.guannengcc.top

now=$(date +%F); echo "$now"
来源：http://all.smart0.xyz

[R27] 算术展开
来源：http://rna.hysaishi.cn

echo $((1 + 2 * 3))
来源：http://jhb.haohaochexian.top

[R28] 浮点运算
来源：http://nad.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://cxp.yuanzhike.top

[R29] 定义函数
来源：http://ntg.fanxiaobao.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xef.jinqigufen.top

[R30] 函数返回状态码
来源：http://zvl.nanxuanxn.top

f() { return 0; }; f || echo "失败了"
来源：http://nnp.0kj1m.cn

[R31] 局部变量
来源：http://sys.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://koj.tanke756.top

[R32] 参数个数校验
来源：http://mug.iojbl.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cus.hywenlv.cn

[R33] 捕获错误并提示行号
来源：http://nvz.zdqjudy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cwg.aizwys.cn

[R34] 退出时清理
来源：http://qhj.wangdashe.top

trap 'rm -f "$tmp"' EXIT
来源：http://bqu.hysaishi.cn

[R35] 后台执行并等待
来源：http://jnu.havefunace.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fly.havefunace.top

[R36] 并发执行多个任务
来源：http://czp.hywenlv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ktw.aibaodan.cn

[R37] 把输出赋给变量
来源：http://jas.epnwcf.com

files=$(ls -1)
来源：http://fnz.pycfn.com

[R38] 管道串联
来源：http://dgc.vqdsnc.cn

cat a.txt | grep -i error | wc -l
来源：http://fbr.cashguo.top

[R39] 重定向标准输出与错误
来源：http://gyc.hesvh.cn

cmd > out.log 2>&1
来源：http://gri.ydzc1.top

[R40] 追加写日志
来源：http://bvx.zhiwuduotai.top

echo "log" >> out.log
来源：http://jad.guowangkeji.top

[R41] 丢弃输出
来源：http://sbo.ivvv.top

cmd >/dev/null 2>&1
来源：http://hwk.tianlin.xyz

[R42] 输入重定向
来源：http://ull.cheryme.top

wc -l < a.txt
来源：http://vvb.shanyushiyangtech.top

[R43] 按名字查找文件
来源：http://mge.jyoumei.cn

find . -name "*.log" -type f
来源：http://lno.fktsv.cn

[R44] 按修改时间查找
来源：http://mla.svipenyu.cn

find . -mtime -7 -type f
来源：http://qle.yanxiufei.cn

[R45] 批量删除
来源：http://ofn.chenlongwang.top

find . -name "*.tmp" -delete
来源：http://hlz.ivvv.top

[R46] 递归替换文件内容
来源：http://ysv.nwbrower.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hio.meibo888.top

[R47] sed 单行替换
来源：http://ipp.fehbvm.com

sed -i 's/foo/bar/g' a.txt
来源：http://ywm.chenzaomai.com

[R48] awk 取指定列
来源：http://nma.zhixingplan.top

awk '{print $1, $3}' a.txt
来源：http://umz.svipenyu.cn

[R49] awk 带条件
来源：http://qsd.hammf.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ukw.havefunace.top

[R50] awk 求和
来源：http://edj.jiagoushi.top

awk '{s += $2} END {print s}' a.txt
来源：http://sdk.kuanghao11.cn

[R51] 排序去重取前几
来源：http://yyy.epnwcf.com

sort a.txt | uniq -c | sort -rn | head
来源：http://uto.yfazqb.com

[R52] 统计行数
来源：http://fjm.gaohongyu789.top

wc -l a.txt
来源：http://qrw.aibaodan.cn

[R53] 查看文件头与实时尾
来源：http://egv.jlsjyb.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pey.yuxming.cn

[R54] 比较两个文件
来源：http://fpx.xziqi.cn

diff a.txt b.txt
来源：http://scg.andypj.xyz

[R55] 压缩与解压
来源：http://hpi.andypj.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hof.zhixingplan.top

[R56] 远程拷贝
来源：http://fox.fengsongda.top

scp file user@host:/path/
来源：http://nhu.fehbvm.com

[R57] 远程执行命令
来源：http://wzw.yueranfly.top

ssh user@host 'uptime'
来源：http://sxn.cucudq.cn

[R58] 下载文件
来源：http://uec.52xcode.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dau.birdmap.top

[R59] 发 POST JSON
来源：http://www.yj20258888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oaq.chenlongwang.top

[R60] 只看 HTTP 状态码
来源：http://evx.gzhubu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oqf.tarul.cn

[R61] 磁盘占用
来源：http://tyr.jlsjyb.cn

df -h;  du -sh *
来源：http://acn.wangdashe.top

[R62] 找最占空间的文件
来源：http://stp.pengpengdd.cyou

du -ah . | sort -rh | head -10
来源：http://vhh.smart0.xyz

[R63] 内存与进程
来源：http://dbo.snrcjt.cn

free -h;  ps aux | grep nginx
来源：http://nhf.jinqigfzy.top

[R64] 结束进程
来源：http://utv.hesvh.cn

kill -9 $(pgrep -f app.py)
来源：http://dgo.redwolf501.top

[R65] 查看端口占用
来源：http://gfj.shanyushiyangtech.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hxe.aibaodan.cn

[R66] 定时任务
来源：http://rxo.pengpengdd.cyou

crontab -e;  crontab -l
来源：http://ilc.yanxiufei.cn

[R67] 生成随机十六进制串
来源：http://swl.birdmap.top

openssl rand -hex 16
来源：http://gyb.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://gow.hysaishi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://oew.cdnleiting.top

[R69] 生成随机密码
来源：http://uwm.fehbvm.com

head -c 16 /dev/urandom | base64
来源：http://zfu.daxiang520.top

[R70] 时间戳与互转
来源：http://vyg.hongshengwenyu.top

date +%s;  date -d @1700000000
来源：http://lob.nanxinkj.top

[R71] 日期格式化
来源：http://ijb.sufxvd.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nac.tian-w.cn

[R72] 等待端口就绪
来源：http://wew.meibo888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zxc.fzhhl.top

[R73] 分割大日志
来源：http://wte.fzhhl.top

split -l 1000 big.log part_
来源：http://flt.jinqigufen.top

[R74] 批量重命名
来源：http://kgt.sufxvd.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mym.yueranfly.top

[R75] 导出环境变量
来源：http://prg.yanxiufei.cn

export PATH="$HOME/bin:$PATH"
来源：http://oug.ehwqpu.com

[R76] 使用临时文件
来源：http://vri.jinqigufen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mdx.jinghuilouyu.cn

[R77] 读取用户输入
来源：http://xoc.gaohongyu789.top

read -rp "请输入: " ans
来源：http://upb.cashguo.top

[R78] 交互式菜单
来源：http://lym.zhixingplan.top

select opt in a b c; do echo "$opt"; break; done
来源：http://nmd.iojbl.cn

[R79] 解析命令行选项
来源：http://zms.ybcxt.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fde.jinqigfzy.top

[R80] 查看脚本执行耗时
来源：http://gvh.zhengqikj.top

time ./run.sh
来源：http://shs.cqqwz.cn

================================================================================
来源：http://pzy.fzhhl.top

S. C / C++ 专题
来源：http://qta.sjlbkw.cn

================================================================================
来源：http://rnp.yangfankeji.com

[S01] C：Hello World
来源：http://zsw.fzhhl.top

#include <stdio.h>
来源：http://fbl.c1oappe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dag.yfazqb.com

[S02] C：变量与格式化输出
来源：http://zjx.haohaochexian.top

int a = 10; printf("%d\n", a);
来源：http://pzs.yanxiufei.cn

[S03] C：读入整数
来源：http://paj.chenzaomai.com

int x; scanf("%d", &x);
来源：http://lbl.zycfv.cn

[S04] C：字符串复制
来源：http://aee.yuxming.cn

char dst[32]; strcpy(dst, "hi");
来源：http://krc.vqdsnc.cn

[S05] C：字符串长度
来源：http://lrd.shzxlz.cn

strlen(s)
来源：http://chn.yj20258888.top

[S06] C：字符串比较
来源：http://irm.hfpthk.cn

strcmp(a, b) == 0
来源：http://feo.zhixingplan.top

[S07] C：数组遍历求和
来源：http://dnk.guowangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://isu.tian-w.cn

[S08] C：动态内存分配与释放
来源：http://xxs.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uct.sweek.top

[S09] C：结构体定义与初始化
来源：http://tzp.shangyingyoupin.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rns.yj202588.top

[S10] C：指针与解引用
来源：http://igs.wangdashe.top

int *p = &a;  *p = 5;
来源：http://dtv.iojbl.cn

[S11] C：逐行读文件
来源：http://rgn.zdbjq.cn

FILE *f = fopen("a.txt", "r");
来源：http://pqz.yfazqb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://sjb.guannengcc.top

fclose(f);
来源：http://qiw.xziqi.cn

[S12] C：写文件
来源：http://tgl.ivvv.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bmy.redwolf501.top

[S13] C：宏定义
来源：http://dgx.sweek.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rsv.zhongyouzk.top

[S14] C：枚举
来源：http://wwj.pengpengdd.cyou

enum Color { RED, GREEN, BLUE };
来源：http://lch.shzxlz.cn

[S15] C：类型转换
来源：http://msy.c1oappe.top

(double) a / b
来源：http://vuo.xylfe.cn

[S16] C：位操作置位
来源：http://tlq.yvedp.cn

x |= (1 << 3);
来源：http://few.feifeiyinyue.top

[S17] C：安全拼接字符串
来源：http://dyd.nanxuanxn.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vqw.dianchejie.cn

[S18] C：命令行参数
来源：http://qle.yanxiufei.cn

int main(int argc, char **argv)
来源：http://brx.ehwqpu.com

[S19] C：快速排序
来源：http://run.aizwys.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xei.cdnleiting.top

[S20] C：二分查找
来源：http://lbv.bbcook.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lrf.xylfe.cn

[S21] C：字符类别判断
来源：http://mjj.vehdjk.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ajg.tarul.cn

[S22] C：字符串转数字
来源：http://umd.haohaochexian.top

atoi("42");  strtod("3.14", NULL);
来源：http://paw.shanyushiyangtech.top

[S23] C：随机数
来源：http://kcy.yvedp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hfk.52xcode.cn

[S24] C：获取本地时间
来源：http://krh.hongshengwenyu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oyw.316326.xyz

[S25] C：内存拷贝
来源：http://nhu.yangfankeji.com

memcpy(dst, src, n);
来源：http://fob.shanyushiyangtech.top

[S26] C：内存清零
来源：http://qrk.guowangkeji.top

memset(a, 0, sizeof a);
来源：http://mji.ywan-chungtsiang.top

[S27] C：定义常量
来源：http://ocz.quarkkingdee.top

const double PI = 3.14159;
来源：http://wqd.ydjk.org.cn

[S28] C：静态变量
来源：http://llj.zycfv.cn

static int counter = 0;
来源：http://mxs.smart0.xyz

[S29] C：变参函数
来源：http://imn.epnwcf.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nwe.52xcode.cn

[S30] C：头文件保护
来源：http://sdd.zhijiandao.cn

#ifndef X_H
来源：http://ftw.shuidangran.top

#define X_H
来源：http://wqw.shzxlz.cn

#endif
来源：http://ppd.zycfv.cn

[S31] C++：Hello World
来源：http://fpy.zhoulong.xyz

#include <iostream>
来源：http://xxr.shangyingyoupin.top

int main() { std::cout << "Hello\n"; }
来源：http://vaf.yongpay.top

[S32] C++：字符串
来源：http://lpn.fanxiaobao.xyz

std::string s = "hi";  s += "!";
来源：http://xvy.hysaishi.cn

[S33] C++：vector 增删
来源：http://kyl.guannengcc.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yzm.yanxiufei.cn

[S34] C++：遍历 vector
来源：http://oec.jinqigfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://zya.ybcxt.top

[S35] C++：map
来源：http://klj.hnqzz.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://icw.zhiwuduotai.top

[S36] C++：unordered_map
来源：http://twp.xinyue.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wwb.yfazqb.com

[S37] C++：set
来源：http://bds.shzxlz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wie.gogol.net.cn

[S38] C++：排序
来源：http://fqn.bjfxy.top

std::sort(v.begin(), v.end());
来源：http://uws.hcnkem.com

[S39] C++：自定义比较器排序
来源：http://uum.jinqigfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iln.uphjek.com

[S40] C++：查找元素
来源：http://xbu.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://frr.bbcook.cn

[S41] C++：类与构造函数
来源：http://fje.guowangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mnn.aibaodan.cn

[S42] C++：继承与虚函数
来源：http://fmm.daria6918.cn

class B : public Base { public: void f() override {} };
来源：http://ixx.zycfv.cn

[S43] C++：智能指针
来源：http://qpw.xinyue.icu

auto p = std::make_unique<int>(5);
来源：http://bun.tanke756.top

[S44] C++：引用传参
来源：http://orw.xinyue.icu

void inc(int &x) { ++x; }
来源：http://umm.tarul.cn

[S45] C++：lambda
来源：http://xmj.ppjwa.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ztv.xuanzx.com

[S46] C++：函数模板
来源：http://oeb.mhx1999.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mmg.jyoumei.cn

[S47] C++：结构化绑定遍历
来源：http://mjr.jinyuanbaomall.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uuu.xinyue.icu

[S48] C++：逐行读文件
来源：http://rjy.smart0.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://gyx.zdqjudy.top

while (std::getline(in, line)) { }
来源：http://snn.xinyue.icu

[S49] C++：写文件
来源：http://wsc.yj202588.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://has.birdmap.top

[S50] C++：格式化数字
来源：http://pqo.gogol.net.cn


<!-- 参考信息 -->