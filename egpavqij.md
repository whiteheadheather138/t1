代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bpt.gaohongyu789.top

[Q75] 日期格式化
来源：http://ngc.ehwqpu.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nwb.jinghuilouyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://njq.yangfankeji.com

[Q76] 按天统计
来源：http://ugs.quarkkingdee.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lmc.pycfn.com

[Q77] 时间加减
来源：http://slo.jqgfzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ehw.jinqigfzy.top

[Q78] 当前时间
来源：http://qmx.fengsongda.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hpw.yueranfly.top

[Q79] 字符串拼接
来源：http://yas.sjlbkw.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ivo.yanxiufei.cn

[Q80] 字符串截取
来源：http://zic.jinyuanbaomall.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dft.andypj.xyz

[Q81] 字符串替换
来源：http://dxi.vqdsnc.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ocl.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://qxy.yonumen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://njv.vehdjk.com

[Q83] 大小写转换
来源：http://eub.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zvn.uphjek.com

[Q84] 去除首尾空格
来源：http://azm.fehbvm.com

SELECT TRIM(name) FROM users;
来源：http://nrf.epnwcf.com

[Q85] 数值取整
来源：http://bie.c1oappe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sfv.xinyue.icu

[Q86] 读取 JSON 字段
来源：http://bfc.9152youxi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wlh.cdnleiting.top

[Q87] JSON 字段做条件
来源：http://cdk.jiagoushi.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lml.dashuyun.cn

[Q88] 行转列（条件聚合）
来源：http://dls.zycfv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qyf.cheryme.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vfd.ivvv.top

[Q89] 判断表是否存在
来源：http://tla.nanxinkj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qft.fehbvm.com

[Q90] 生成序号列
来源：http://wjj.guannengcc.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bdy.yangfankeji.com

================================================================================
来源：http://yyp.fengsongda.top

R. Bash 专题
来源：http://ojl.hesvh.cn

================================================================================
来源：http://tfo.52xcode.cn

[R01] shebang 与严格模式
来源：http://sfk.shanyushiyangtech.top

#!/usr/bin/env bash
来源：http://spi.zhaomingkeji.xyz

set -euo pipefail
来源：http://fkq.jiagoushi.top

[R02] 变量赋值与使用
来源：http://aqq.daria6918.cn

name="Tom"; echo "$name"
来源：http://ihz.hysaishi.cn

[R03] 只读变量
来源：http://apm.zdbjq.cn

readonly PI=3.14
来源：http://rae.ybcxt.top

[R04] 位置参数
来源：http://enq.shangyingyoupin.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sdr.fanxiaobao.xyz

[R05] 参数默认值
来源：http://kwh.feifeiyinyue.top

name="${1:-default}"
来源：http://wzm.gzhubu.top

[R06] 判断命令是否存在
来源：http://kve.hfpthk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xfa.dianchejie.cn

[R07] if 判断文件
来源：http://pmy.9152youxi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tdf.jinyuanbaomall.cn

[R08] 数值比较
来源：http://znb.nanxinkj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hno.havefunace.top

[R09] 字符串比较
来源：http://dtn.chenzaomai.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vpz.tianlin.xyz

[R10] 正则匹配
来源：http://ign.gzhubu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lwp.zycfv.cn

[R11] case 多分支
来源：http://zyw.tian-w.cn

case "$1" in
来源：http://xmw.nanxuanxn.top

start) echo "启动" ;;
来源：http://sty.guowangkeji.top

stop)  echo "停止" ;;
来源：http://dgc.zhixingplan.top

*)     echo "未知命令" ;;
来源：http://hvk.cdnleiting.top

esac
来源：http://zzn.xziqi.cn

[R12] for 遍历文件
来源：http://ube.daxiang520.top

for f in *.txt; do echo "$f"; done
来源：http://jbz.yj20258888.top

[R13] for 计数循环
来源：http://hkg.shzxlz.cn

for i in {1..10}; do echo "$i"; done
来源：http://mbp.vqdsnc.cn

[R14] C 风格 for
来源：http://rdd.jinyuanbaomall.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ggj.gotoacloud.top

[R15] while 逐行读文件
来源：http://nie.xingfuxueyuan.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://amg.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://oci.feifeiyinyue.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dlb.nwbrower.top

[R17] 数组定义与取值
来源：http://kit.jianghu66.top

arr=(a b c); echo "${arr[0]}"
来源：http://gru.andypj.xyz

[R18] 遍历数组
来源：http://olz.fehbvm.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hmm.iojbl.cn

[R19] 数组长度
来源：http://pbe.zhaomingkeji.xyz

echo "${#arr[@]}"
来源：http://ndl.jinqigfzy.top

[R20] 关联数组（字典）
来源：http://fqu.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zro.shangyingyoupin.top

[R21] 字符串长度
来源：http://vmk.fktsv.cn

echo "${#s}"
来源：http://khz.jinqigufen.top

[R22] 截取子串
来源：http://flk.xuanzx.com

echo "${s:0:5}"
来源：http://vjy.yangfankeji.com

[R23] 字符串替换
来源：http://trs.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vwm.gaohongyu789.top

[R24] 大小写转换
来源：http://zym.sweek.top

echo "${s^^}"; echo "${s,,}"
来源：http://zsf.hammf.cn

[R25] 去后缀 / 去前缀
来源：http://chk.xingfuxueyuan.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://xcw.fehbvm.com

[R26] 命令替换
来源：http://lrs.fanxiaobao.xyz

now=$(date +%F); echo "$now"
来源：http://roz.pengpengdd.cyou

[R27] 算术展开
来源：http://bix.jyoumei.cn

echo $((1 + 2 * 3))
来源：http://jin.jinghuilouyu.cn

[R28] 浮点运算
来源：http://mnc.jqgufenzy.top

echo "scale=2; 10/3" | bc
来源：http://syp.cheryme.top

[R29] 定义函数
来源：http://tjv.pycfn.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gca.ywan-chungtsiang.top

[R30] 函数返回状态码
来源：http://okw.tianlin.xyz

f() { return 0; }; f || echo "失败了"
来源：http://meq.shangyingyoupin.top

[R31] 局部变量
来源：http://dnf.ybcxt.top

f() { local x=1; echo "$x"; }
来源：http://pjk.jianghu66.top

[R32] 参数个数校验
来源：http://tqg.bjfxy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qsy.nwbrower.top

[R33] 捕获错误并提示行号
来源：http://zik.cqqwz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bqh.vehdjk.com

[R34] 退出时清理
来源：http://ocu.gotoacloud.top

trap 'rm -f "$tmp"' EXIT
来源：http://uxw.fanxiaobao.xyz

[R35] 后台执行并等待
来源：http://jxk.dashuyun.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uyh.xingfuxueyuan.xyz

[R36] 并发执行多个任务
来源：http://djg.hcnkem.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gzb.hnqzz.top

[R37] 把输出赋给变量
来源：http://txp.svipenyu.cn

files=$(ls -1)
来源：http://pza.pycfn.com

[R38] 管道串联
来源：http://plu.hywenlv.cn

cat a.txt | grep -i error | wc -l
来源：http://ihd.fanxiaobao.xyz

[R39] 重定向标准输出与错误
来源：http://nzt.yonumen.top

cmd > out.log 2>&1
来源：http://swr.nanxinkj.top

[R40] 追加写日志
来源：http://mfi.bjfxy.top

echo "log" >> out.log
来源：http://eej.aizwys.cn

[R41] 丢弃输出
来源：http://lyk.ctjpmb.com

cmd >/dev/null 2>&1
来源：http://urf.sjlbkw.cn

[R42] 输入重定向
来源：http://xrv.yuxming.cn

wc -l < a.txt
来源：http://hgl.fehbvm.com

[R43] 按名字查找文件
来源：http://www.ivvv.top

find . -name "*.log" -type f
来源：http://qhr.316326.xyz

[R44] 按修改时间查找
来源：http://yvl.hammf.cn

find . -mtime -7 -type f
来源：http://cgh.uphjek.com

[R45] 批量删除
来源：http://sqi.ivvv.top

find . -name "*.tmp" -delete
来源：http://aoe.jinqigfzy.top

[R46] 递归替换文件内容
来源：http://hiu.sweek.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bfc.tian-w.cn

[R47] sed 单行替换
来源：http://kkj.xziqi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vqc.sysykeji.top

[R48] awk 取指定列
来源：http://zll.hongshengwenyu.top

awk '{print $1, $3}' a.txt
来源：http://mtc.svipenyu.cn

[R49] awk 带条件
来源：http://ljl.tarul.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://txg.guowangkeji.top

[R50] awk 求和
来源：http://fzy.hnxiangtu.top

awk '{s += $2} END {print s}' a.txt
来源：http://avm.xylfe.cn

[R51] 排序去重取前几
来源：http://usj.pengpengdd.cyou

sort a.txt | uniq -c | sort -rn | head
来源：http://cuy.svipenyu.cn

[R52] 统计行数
来源：http://frf.yanxiufei.cn

wc -l a.txt
来源：http://qse.cheryme.top

[R53] 查看文件头与实时尾
来源：http://zqu.shuidangran.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mef.shanyushiyangkeji.top

[R54] 比较两个文件
来源：http://dyn.zhaomingkeji.xyz

diff a.txt b.txt
来源：http://fwt.hnqzz.top

[R55] 压缩与解压
来源：http://vgr.cheryme.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://chs.chenlongwang.top

[R56] 远程拷贝
来源：http://dlq.daxiang520.top

scp file user@host:/path/
来源：http://xnk.guannengcc.top

[R57] 远程执行命令
来源：http://pmh.0kj1m.cn

ssh user@host 'uptime'
来源：http://pvx.ywan-chungtsiang.top

[R58] 下载文件
来源：http://hxz.hysaishi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wza.sysykeji.top

[R59] 发 POST JSON
来源：http://gfg.ivvv.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gen.xuanzx.com

[R60] 只看 HTTP 状态码
来源：http://hlx.gogol.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cur.ydzc1.top

[R61] 磁盘占用
来源：http://pfo.shanyushiyangtech.top

df -h;  du -sh *
来源：http://xev.uphjek.com

[R62] 找最占空间的文件
来源：http://jqw.shzxlz.cn

du -ah . | sort -rh | head -10
来源：http://kaq.chenjidiqi.icu

[R63] 内存与进程
来源：http://cnq.cashguo.top

free -h;  ps aux | grep nginx
来源：http://vaw.shangyingyoupin.top

[R64] 结束进程
来源：http://dhk.fzhhl.top

kill -9 $(pgrep -f app.py)
来源：http://nwr.xylfe.cn

[R65] 查看端口占用
来源：http://khg.tianlin.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qpd.yueranfly.top

[R66] 定时任务
来源：http://fig.jinghuilouyu.cn

crontab -e;  crontab -l
来源：http://dqb.zdbjq.cn

[R67] 生成随机十六进制串
来源：http://hjf.tarul.cn

openssl rand -hex 16
来源：http://lkv.yuanzhike.top

[R68] 计算文件校验值
来源：http://nxa.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://eap.zhoulong.xyz

[R69] 生成随机密码
来源：http://inh.hcnkem.com

head -c 16 /dev/urandom | base64
来源：http://itc.ybcxt.top

[R70] 时间戳与互转
来源：http://oms.yongpay.top

date +%s;  date -d @1700000000
来源：http://tpc.fehbvm.com

[R71] 日期格式化
来源：http://mfd.cqqwz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lei.mhx1999.top

[R72] 等待端口就绪
来源：http://gmr.aizwys.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lmy.daxiang520.top

[R73] 分割大日志
来源：http://kml.zhaomingkeji.xyz

split -l 1000 big.log part_
来源：http://kvx.pengpengdd.cyou

[R74] 批量重命名
来源：http://hfy.cucudq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gwt.jyoumei.cn

[R75] 导出环境变量
来源：http://ymx.hongshengwenyu.top

export PATH="$HOME/bin:$PATH"
来源：http://rkj.yangfankeji.com

[R76] 使用临时文件
来源：http://nsi.gogol.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lil.ppjwa.cn

[R77] 读取用户输入
来源：http://ial.smart0.xyz

read -rp "请输入: " ans
来源：http://gjz.shanyushiyangkeji.top

[R78] 交互式菜单
来源：http://rdd.xylfe.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://aja.hcnkem.com

[R79] 解析命令行选项
来源：http://yok.hongshengwenyu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uyg.jyoumei.cn

[R80] 查看脚本执行耗时
来源：http://xqn.jinqigufen.top

time ./run.sh
来源：http://tkb.cashguo.top

================================================================================
来源：http://dxf.zhijiandao.cn

S. C / C++ 专题
来源：http://wgn.yvedp.cn

================================================================================
来源：http://pyh.snrcjt.cn

[S01] C：Hello World
来源：http://ypq.fehbvm.com

#include <stdio.h>
来源：http://ikw.dashuyun.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zyo.quarkkingdee.top

[S02] C：变量与格式化输出
来源：http://rtb.dashuyun.cn

int a = 10; printf("%d\n", a);
来源：http://rhl.hfpthk.cn

[S03] C：读入整数
来源：http://hbj.yueranfly.top

int x; scanf("%d", &x);
来源：http://kyu.sysykeji.top

[S04] C：字符串复制
来源：http://mqs.ppjwa.cn

char dst[32]; strcpy(dst, "hi");
来源：http://iun.ppjwa.cn

[S05] C：字符串长度
来源：http://hiu.tarul.cn

strlen(s)
来源：http://yhk.snrcjt.cn

[S06] C：字符串比较
来源：http://fio.zhijiandao.cn

strcmp(a, b) == 0
来源：http://hwc.snrcjt.cn

[S07] C：数组遍历求和
来源：http://ikt.52xcode.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rlb.shangyingyoupin.top

[S08] C：动态内存分配与释放
来源：http://kbl.ydjk.org.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qlw.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://etx.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bzr.jinyuanbaomall.cn

[S10] C：指针与解引用
来源：http://tpw.nwbrower.top

int *p = &a;  *p = 5;
来源：http://sgg.tanke756.top

[S11] C：逐行读文件
来源：http://kpv.fzhhl.top

FILE *f = fopen("a.txt", "r");
来源：http://rqz.gotoacloud.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://luv.havefunace.top

fclose(f);
来源：http://zsh.yfazqb.com

[S12] C：写文件
来源：http://agv.hcnkem.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ewz.sufxvd.cn

[S13] C：宏定义
来源：http://ika.pengpengdd.cyou

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mee.cucudq.cn

[S14] C：枚举
来源：http://wvu.xingfuxueyuan.xyz

enum Color { RED, GREEN, BLUE };
来源：http://hbo.jinyuanbaomall.cn

[S15] C：类型转换
来源：http://rlk.jinqigufen.top

(double) a / b
来源：http://uky.havefunace.top

[S16] C：位操作置位
来源：http://low.jianghu66.top

x |= (1 << 3);
来源：http://nzq.jqgufenzy.top

[S17] C：安全拼接字符串
来源：http://lat.aizwys.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://azt.uphjek.com

[S18] C：命令行参数
来源：http://cbd.hnxiangtu.top

int main(int argc, char **argv)
来源：http://gpt.fengsongda.top

[S19] C：快速排序
来源：http://jvw.jinqigfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://yhf.yonumen.top

[S20] C：二分查找
来源：http://cev.fktsv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ise.xinyue.icu

[S21] C：字符类别判断
来源：http://nrw.zdbjq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://akf.jianghu66.top

[S22] C：字符串转数字
来源：http://pij.zhongyouzk.top

atoi("42");  strtod("3.14", NULL);
来源：http://onk.gogol.net.cn

[S23] C：随机数
来源：http://rtf.0kj1m.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://elm.yvedp.cn

[S24] C：获取本地时间
来源：http://ryq.cdnleiting.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bfw.yongpay.top

[S25] C：内存拷贝
来源：http://bte.vehdjk.com

memcpy(dst, src, n);
来源：http://jmg.uphjek.com

[S26] C：内存清零
来源：http://avn.zdqjudy.top

memset(a, 0, sizeof a);
来源：http://pwh.svipenyu.cn

[S27] C：定义常量
来源：http://mcb.jqgufenzy.top

const double PI = 3.14159;
来源：http://umv.sufxvd.cn

[S28] C：静态变量
来源：http://sgm.zhongyouzk.top

static int counter = 0;
来源：http://ihm.havefunace.top

[S29] C：变参函数
来源：http://esh.ydzc1.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hkt.bjfxy.top

[S30] C：头文件保护
来源：http://evw.hnxiangtu.top

#ifndef X_H
来源：http://cxh.zhiwuduotai.top

#define X_H
来源：http://gqz.epnwcf.com

#endif
来源：http://xih.kuanghao11.cn

[S31] C++：Hello World
来源：http://ldc.hywenlv.cn

#include <iostream>
来源：http://oec.jqgufenzy.top

int main() { std::cout << "Hello\n"; }
来源：http://bnb.gogol.net.cn

[S32] C++：字符串
来源：http://oun.havefunace.top

std::string s = "hi";  s += "!";
来源：http://pjf.snrcjt.cn

[S33] C++：vector 增删
来源：http://riw.9152youxi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ntu.hesvh.cn

[S34] C++：遍历 vector
来源：http://zzf.snrcjt.cn

for (auto &x : v) { std::cout << x; }
来源：http://yab.bbcook.cn

[S35] C++：map
来源：http://jjj.jyoumei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tsd.ybcxt.top

[S36] C++：unordered_map
来源：http://sgt.jlsjyb.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://udv.ydjk.org.cn

[S37] C++：set
来源：http://wrk.yanxiufei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mob.pycfn.com

[S38] C++：排序
来源：http://xyu.nwbrower.top

std::sort(v.begin(), v.end());
来源：http://nsc.tianlin.xyz

[S39] C++：自定义比较器排序
来源：http://laz.gogol.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://swb.daxiang520.top

[S40] C++：查找元素
来源：http://ubx.chenzaomai.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jnm.svipenyu.cn

[S41] C++：类与构造函数
来源：http://kbi.yueranfly.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dnw.jinqigfzy.top

[S42] C++：继承与虚函数
来源：http://its.jiagoushi.top

class B : public Base { public: void f() override {} };
来源：http://pgu.wangshuangyany.cn

[S43] C++：智能指针
来源：http://gtq.hfpthk.cn

auto p = std::make_unique<int>(5);
来源：http://ook.yj20258888.top

[S44] C++：引用传参
来源：http://ksf.guowangkeji.top

void inc(int &x) { ++x; }
来源：http://nle.guowangkeji.top


<!-- 参考信息 -->