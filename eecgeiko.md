代发 wailian999

[Q76] 按天统计
来源：http://wiz.nanxuanxn.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://orz.vehdjk.com

[Q77] 时间加减
来源：http://zbh.nwbrower.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qqg.sjlbkw.cn

[Q78] 当前时间
来源：http://fus.hysaishi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rgr.yfazqb.com

[Q79] 字符串拼接
来源：http://glj.yangfankeji.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gqp.52xcode.cn

[Q80] 字符串截取
来源：http://pfh.shuidangran.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://okn.yangfankeji.com

[Q81] 字符串替换
来源：http://yhe.fanxiaobao.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wou.yangfankeji.com

[Q82] 字符长度与字节长度
来源：http://aid.hongshengwenyu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kcy.jiagoushi.top

[Q83] 大小写转换
来源：http://dgy.gaohongyu789.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cum.svipenyu.cn

[Q84] 去除首尾空格
来源：http://rhq.sxryk.cn

SELECT TRIM(name) FROM users;
来源：http://lll.bjfxy.top

[Q85] 数值取整
来源：http://ntp.xingfuxueyuan.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://clj.xylfe.cn

[Q86] 读取 JSON 字段
来源：http://wlw.xziqi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fur.gotoacloud.top

[Q87] JSON 字段做条件
来源：http://qbc.cheryme.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://loz.guowangkeji.top

[Q88] 行转列（条件聚合）
来源：http://mwx.tanke756.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zfc.zdbjq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tvb.hfpthk.cn

[Q89] 判断表是否存在
来源：http://nof.quarkkingdee.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mqe.tianlin.xyz

[Q90] 生成序号列
来源：http://eqz.nwbrower.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tkm.wangdashe.top

================================================================================
来源：http://whu.yvedp.cn

R. Bash 专题
来源：http://vyt.xziqi.cn

================================================================================
来源：http://eyl.sjlbkw.cn

[R01] shebang 与严格模式
来源：http://for.bjfxy.top

#!/usr/bin/env bash
来源：http://xxu.quarkkingdee.top

set -euo pipefail
来源：http://ree.jinghuilouyu.cn

[R02] 变量赋值与使用
来源：http://tdi.sxryk.cn

name="Tom"; echo "$name"
来源：http://sxs.guannengcc.top

[R03] 只读变量
来源：http://nbi.epnwcf.com

readonly PI=3.14
来源：http://vca.pycfn.com

[R04] 位置参数
来源：http://ltz.hammf.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qpe.yangfankeji.com

[R05] 参数默认值
来源：http://aes.redwolf501.top

name="${1:-default}"
来源：http://ajx.ehwqpu.com

[R06] 判断命令是否存在
来源：http://fzq.hnxiangtu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://suj.52xcode.cn

[R07] if 判断文件
来源：http://fjw.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dqb.nwbrower.top

[R08] 数值比较
来源：http://mez.tianlin.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://jno.pycfn.com

[R09] 字符串比较
来源：http://tcl.jiagoushi.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hes.yuxming.cn

[R10] 正则匹配
来源：http://mhk.nanxinkj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lfl.wangshuangyany.cn

[R11] case 多分支
来源：http://ihz.zhengqikj.top

case "$1" in
来源：http://hyr.hywenlv.cn

start) echo "启动" ;;
来源：http://rwf.hnxiangtu.top

stop)  echo "停止" ;;
来源：http://iow.ydjk.org.cn

*)     echo "未知命令" ;;
来源：http://fhq.zhoulong.xyz

esac
来源：http://xbo.jinqigfzy.top

[R12] for 遍历文件
来源：http://udz.shanyushiyangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://acv.smart0.xyz

[R13] for 计数循环
来源：http://fra.yanxiufei.cn

for i in {1..10}; do echo "$i"; done
来源：http://eaf.zhengqikj.top

[R14] C 风格 for
来源：http://lxf.svipenyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ztb.chenlongwang.top

[R15] while 逐行读文件
来源：http://jyf.jqgfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ofc.dianchejie.cn

[R16] until 等待条件
来源：http://giu.ppjwa.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wnq.kuanghao11.cn

[R17] 数组定义与取值
来源：http://byo.svipenyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dsl.svipenyu.cn

[R18] 遍历数组
来源：http://rkr.yfazqb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ixc.yongpay.top

[R19] 数组长度
来源：http://osk.jlsjyb.cn

echo "${#arr[@]}"
来源：http://dbx.vqdsnc.cn

[R20] 关联数组（字典）
来源：http://wyg.xuetiantiany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wsj.pycfn.com

[R21] 字符串长度
来源：http://grc.cqqwz.cn

echo "${#s}"
来源：http://nsk.jinqigfzy.top

[R22] 截取子串
来源：http://cgo.ctjpmb.com

echo "${s:0:5}"
来源：http://vsf.yueranfly.top

[R23] 字符串替换
来源：http://zab.iojbl.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yis.yuxming.cn

[R24] 大小写转换
来源：http://cvu.chenlongwang.top

echo "${s^^}"; echo "${s,,}"
来源：http://moy.cashguo.top

[R25] 去后缀 / 去前缀
来源：http://ipy.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://blg.cqqwz.cn

[R26] 命令替换
来源：http://zkj.sysykeji.top

now=$(date +%F); echo "$now"
来源：http://eme.dashuyun.cn

[R27] 算术展开
来源：http://vxr.yj20258888.top

echo $((1 + 2 * 3))
来源：http://kik.vehdjk.com

[R28] 浮点运算
来源：http://qra.hfpthk.cn

echo "scale=2; 10/3" | bc
来源：http://ntj.cucudq.cn

[R29] 定义函数
来源：http://ffw.ctjpmb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qvx.cucudq.cn

[R30] 函数返回状态码
来源：http://tvw.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://lge.pycfn.com

[R31] 局部变量
来源：http://bhj.zhoulong.xyz

f() { local x=1; echo "$x"; }
来源：http://hjr.xinyue.icu

[R32] 参数个数校验
来源：http://fmw.jinqigufen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qke.xziqi.cn

[R33] 捕获错误并提示行号
来源：http://xaa.cdnleiting.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ute.gotoacloud.top

[R34] 退出时清理
来源：http://wih.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://hkl.yfazqb.com

[R35] 后台执行并等待
来源：http://vsm.jyoumei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kyu.yongpay.top

[R36] 并发执行多个任务
来源：http://eps.hnqzz.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nhm.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://feg.daxiang520.top

files=$(ls -1)
来源：http://zds.bjfxy.top

[R38] 管道串联
来源：http://kio.daria6918.cn

cat a.txt | grep -i error | wc -l
来源：http://olp.dianchejie.cn

[R39] 重定向标准输出与错误
来源：http://qhc.yvedp.cn

cmd > out.log 2>&1
来源：http://yaz.zhixingplan.top

[R40] 追加写日志
来源：http://jub.9152youxi.cn

echo "log" >> out.log
来源：http://rlr.redwolf501.top

[R41] 丢弃输出
来源：http://vem.kuanghao11.cn

cmd >/dev/null 2>&1
来源：http://ped.quarkkingdee.top

[R42] 输入重定向
来源：http://fhd.tianlin.xyz

wc -l < a.txt
来源：http://azy.ppjwa.cn

[R43] 按名字查找文件
来源：http://vko.yj202588.top

find . -name "*.log" -type f
来源：http://yrh.guowangkeji.top

[R44] 按修改时间查找
来源：http://eqk.hcnkem.com

find . -mtime -7 -type f
来源：http://xgi.c1oappe.top

[R45] 批量删除
来源：http://tls.fengsongda.top

find . -name "*.tmp" -delete
来源：http://rfd.chenlongwang.top

[R46] 递归替换文件内容
来源：http://gsq.gaohongyu789.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gch.gogol.net.cn

[R47] sed 单行替换
来源：http://jov.daria6918.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ddq.aizwys.cn

[R48] awk 取指定列
来源：http://rlg.epnwcf.com

awk '{print $1, $3}' a.txt
来源：http://uqg.xuetiantiany.cn

[R49] awk 带条件
来源：http://rgg.svipenyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sxp.jinghuilouyu.cn

[R50] awk 求和
来源：http://erg.yuxming.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wxt.uphjek.com

[R51] 排序去重取前几
来源：http://jdc.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oym.havefunace.top

[R52] 统计行数
来源：http://syr.zhaomingkeji.xyz

wc -l a.txt
来源：http://iaf.ydzc1.top

[R53] 查看文件头与实时尾
来源：http://ftl.uphjek.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://elr.hesvh.cn

[R54] 比较两个文件
来源：http://xpr.sxryk.cn

diff a.txt b.txt
来源：http://meq.zdbjq.cn

[R55] 压缩与解压
来源：http://meb.zhaomingkeji.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zcb.kuanghao11.cn

[R56] 远程拷贝
来源：http://bxd.vqdsnc.cn

scp file user@host:/path/
来源：http://vhw.316326.xyz

[R57] 远程执行命令
来源：http://afu.ydjk.org.cn

ssh user@host 'uptime'
来源：http://fym.svipenyu.cn

[R58] 下载文件
来源：http://oap.yuxming.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wuz.bjfxy.top

[R59] 发 POST JSON
来源：http://ple.yj202588.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pjg.cashguo.top

[R60] 只看 HTTP 状态码
来源：http://ppj.hnxiangtu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rdu.yvedp.cn

[R61] 磁盘占用
来源：http://jtu.wangshuangyany.cn

df -h;  du -sh *
来源：http://vve.tianlin.xyz

[R62] 找最占空间的文件
来源：http://ych.zycfv.cn

du -ah . | sort -rh | head -10
来源：http://uzm.shzxlz.cn

[R63] 内存与进程
来源：http://rhz.feifeiyinyue.top

free -h;  ps aux | grep nginx
来源：http://zps.pengpengdd.cyou

[R64] 结束进程
来源：http://uxt.jqgufenzy.top

kill -9 $(pgrep -f app.py)
来源：http://ccb.chenlongwang.top

[R65] 查看端口占用
来源：http://ulf.zycfv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rvo.jinqigufen.top

[R66] 定时任务
来源：http://vaq.yvedp.cn

crontab -e;  crontab -l
来源：http://fyj.zhixingplan.top

[R67] 生成随机十六进制串
来源：http://blx.yj20258.top

openssl rand -hex 16
来源：http://qkn.yj20258888.top

[R68] 计算文件校验值
来源：http://kpe.316326.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://diu.daria6918.cn

[R69] 生成随机密码
来源：http://wkx.jqgufenzy.top

head -c 16 /dev/urandom | base64
来源：http://luq.yonumen.top

[R70] 时间戳与互转
来源：http://qrp.yonumen.top

date +%s;  date -d @1700000000
来源：http://out.bjfxy.top

[R71] 日期格式化
来源：http://dxz.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bho.zycfv.cn

[R72] 等待端口就绪
来源：http://hqg.fktsv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dip.jqgufenzy.top

[R73] 分割大日志
来源：http://yih.zhijiandao.cn

split -l 1000 big.log part_
来源：http://tyy.smart0.xyz

[R74] 批量重命名
来源：http://lof.tarul.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ffl.havefunace.top

[R75] 导出环境变量
来源：http://mfr.guannengcc.top

export PATH="$HOME/bin:$PATH"
来源：http://zrw.yonumen.top

[R76] 使用临时文件
来源：http://mli.yvedp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://elx.cdnleiting.top

[R77] 读取用户输入
来源：http://zui.bbcook.cn

read -rp "请输入: " ans
来源：http://qgr.zdbjq.cn

[R78] 交互式菜单
来源：http://oiv.hcnkem.com

select opt in a b c; do echo "$opt"; break; done
来源：http://pvv.guowangkeji.top

[R79] 解析命令行选项
来源：http://vvv.gogol.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://shp.feifeiyinyue.top

[R80] 查看脚本执行耗时
来源：http://ifh.zhijiandao.cn

time ./run.sh
来源：http://kzh.guannengcc.top

================================================================================
来源：http://tlm.xinyue.icu

S. C / C++ 专题
来源：http://deq.yanxiufei.cn

================================================================================
来源：http://exh.daria6918.cn

[S01] C：Hello World
来源：http://aiz.tian-w.cn

#include <stdio.h>
来源：http://bgm.xylfe.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ngk.c1oappe.top

[S02] C：变量与格式化输出
来源：http://uwe.dashuyun.cn

int a = 10; printf("%d\n", a);
来源：http://cwy.xylfe.cn

[S03] C：读入整数
来源：http://irb.zycfv.cn

int x; scanf("%d", &x);
来源：http://ejx.cashguo.top

[S04] C：字符串复制
来源：http://znv.jinqigufen.top

char dst[32]; strcpy(dst, "hi");
来源：http://opd.yueranfly.top

[S05] C：字符串长度
来源：http://ytr.jiagoushi.top

strlen(s)
来源：http://tyg.shanyushiyangtech.top

[S06] C：字符串比较
来源：http://kwi.yanxiufei.cn

strcmp(a, b) == 0
来源：http://ytt.hysaishi.cn

[S07] C：数组遍历求和
来源：http://xjp.bbcook.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pbs.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://cap.daxiang520.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vit.ywan-chungtsiang.top

[S09] C：结构体定义与初始化
来源：http://rzp.sxryk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cpt.nwbrower.top

[S10] C：指针与解引用
来源：http://dnc.daria6918.cn

int *p = &a;  *p = 5;
来源：http://dst.chenlongwang.top

[S11] C：逐行读文件
来源：http://xuc.chenjidiqi.icu

FILE *f = fopen("a.txt", "r");
来源：http://fos.chenzaomai.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://mmv.havefunace.top

fclose(f);
来源：http://jmo.hesvh.cn

[S12] C：写文件
来源：http://ckg.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rzc.havefunace.top

[S13] C：宏定义
来源：http://hrk.tianlin.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jvy.haohaochexian.top

[S14] C：枚举
来源：http://yte.ydzc1.top

enum Color { RED, GREEN, BLUE };
来源：http://cgl.jiagoushi.top

[S15] C：类型转换
来源：http://nlu.bbcook.cn

(double) a / b
来源：http://dnz.tian-w.cn

[S16] C：位操作置位
来源：http://dms.gotoacloud.top

x |= (1 << 3);
来源：http://uzj.gotoacloud.top

[S17] C：安全拼接字符串
来源：http://dtt.xuetiantiany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hws.tianlin.xyz

[S18] C：命令行参数
来源：http://pxc.cheryme.top

int main(int argc, char **argv)
来源：http://tto.fengsongda.top

[S19] C：快速排序
来源：http://oor.wangdashe.top

qsort(a, n, sizeof(int), cmp);
来源：http://fne.xinyue.icu

[S20] C：二分查找
来源：http://akl.cheryme.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nwz.fktsv.cn

[S21] C：字符类别判断
来源：http://tct.yj20258888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wqc.hnqzz.top

[S22] C：字符串转数字
来源：http://vsp.jinqigfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://wjt.chenlongwang.top

[S23] C：随机数
来源：http://lqx.pengpengdd.cyou

srand(time(NULL));  int r = rand() % 100;
来源：http://blv.dashuyun.cn

[S24] C：获取本地时间
来源：http://lzk.jqgfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mqv.cqqwz.cn

[S25] C：内存拷贝
来源：http://sbs.0kj1m.cn

memcpy(dst, src, n);
来源：http://sbd.yj202588.top

[S26] C：内存清零
来源：http://uif.vehdjk.com

memset(a, 0, sizeof a);
来源：http://dig.feifeiyinyue.top

[S27] C：定义常量
来源：http://ocd.yuanzhike.top

const double PI = 3.14159;
来源：http://ujn.xziqi.cn

[S28] C：静态变量
来源：http://bxe.epnwcf.com

static int counter = 0;
来源：http://nke.52xcode.cn

[S29] C：变参函数
来源：http://net.bbcook.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pye.zhijiandao.cn

[S30] C：头文件保护
来源：http://dql.jqgufenzy.top

#ifndef X_H
来源：http://qvm.jianghu66.top

#define X_H
来源：http://dmv.jinqigufen.top

#endif
来源：http://orl.chenzaomai.com

[S31] C++：Hello World
来源：http://dtv.daria6918.cn

#include <iostream>
来源：http://gdz.cashguo.top

int main() { std::cout << "Hello\n"; }
来源：http://uoq.sufxvd.cn

[S32] C++：字符串
来源：http://fxa.cucudq.cn

std::string s = "hi";  s += "!";
来源：http://lvc.epnwcf.com

[S33] C++：vector 增删
来源：http://smv.zhongyouzk.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://szf.hnqzz.top

[S34] C++：遍历 vector
来源：http://meo.nanxinkj.top

for (auto &x : v) { std::cout << x; }
来源：http://hyx.fengsongda.top

[S35] C++：map
来源：http://iop.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vrs.gotoacloud.top

[S36] C++：unordered_map
来源：http://tpp.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://akt.vqdsnc.cn

[S37] C++：set
来源：http://bpb.jyoumei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xgs.hongshengwenyu.top

[S38] C++：排序
来源：http://qbj.jinqigfzy.top

std::sort(v.begin(), v.end());
来源：http://tqb.shuidangran.top

[S39] C++：自定义比较器排序
来源：http://ghy.hongshengwenyu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bjs.316326.xyz

[S40] C++：查找元素
来源：http://qmt.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://glx.jyoumei.cn

[S41] C++：类与构造函数
来源：http://ewk.fanxiaobao.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ocv.gogol.net.cn

[S42] C++：继承与虚函数
来源：http://zmt.gogol.net.cn

class B : public Base { public: void f() override {} };
来源：http://rlf.andypj.xyz

[S43] C++：智能指针
来源：http://olm.xinyue.icu

auto p = std::make_unique<int>(5);
来源：http://aqc.birdmap.top

[S44] C++：引用传参
来源：http://cor.wangdashe.top

void inc(int &x) { ++x; }
来源：http://lpu.9152youxi.cn

[S45] C++：lambda
来源：http://idq.shanyushiyangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://ufr.ehwqpu.com

[S46] C++：函数模板
来源：http://mzp.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jmd.andypj.xyz


<!-- 参考信息 -->