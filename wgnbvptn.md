代发 wailian999

ANALYZE TABLE users;
来源：http://jde.meibo888.top

[Q71] 查看建表语句
来源：http://hct.epnwcf.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ibt.shangyingyoupin.top

[Q72] 查看索引
来源：http://wki.andypj.xyz

SHOW INDEX FROM users;
来源：http://oei.ehwqpu.com

[Q73] 查看表状态
来源：http://icx.vehdjk.com

SHOW TABLE STATUS LIKE 'users';
来源：http://mgz.ybcxt.top

[Q74] 强制使用索引
来源：http://evs.yj20258888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dto.tian-w.cn

[Q75] 日期格式化
来源：http://avj.jqgfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dlv.fanxiaobao.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dlf.ydzc1.top

[Q76] 按天统计
来源：http://xjt.pycfn.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://awc.wangdashe.top

[Q77] 时间加减
来源：http://bfp.yanxiufei.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dmr.ivvv.top

[Q78] 当前时间
来源：http://rmz.shanyushiyangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xho.wangdashe.top

[Q79] 字符串拼接
来源：http://jou.fktsv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://idn.vehdjk.com

[Q80] 字符串截取
来源：http://efy.fehbvm.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bvd.aibaodan.cn

[Q81] 字符串替换
来源：http://sbm.uphjek.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mzq.fehbvm.com

[Q82] 字符长度与字节长度
来源：http://vrr.havefunace.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nat.dashuyun.cn

[Q83] 大小写转换
来源：http://ppv.zhengqikj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ymq.yuxming.cn

[Q84] 去除首尾空格
来源：http://bbg.jqgfzy.top

SELECT TRIM(name) FROM users;
来源：http://dtx.daria6918.cn

[Q85] 数值取整
来源：http://dsh.shanyushiyangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gdg.jianghu66.top

[Q86] 读取 JSON 字段
来源：http://isy.sweek.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ofh.gaohongyu789.top

[Q87] JSON 字段做条件
来源：http://wqb.feifeiyinyue.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tez.vehdjk.com

[Q88] 行转列（条件聚合）
来源：http://rpg.chenzaomai.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ynk.xylfe.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gxd.shanyushiyangkeji.top

[Q89] 判断表是否存在
来源：http://bxa.sxryk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gce.hnqzz.top

[Q90] 生成序号列
来源：http://mex.jlsjyb.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pyt.c1oappe.top

================================================================================
来源：http://lkb.xziqi.cn

R. Bash 专题
来源：http://rfw.zhoulong.xyz

================================================================================
来源：http://gap.jinyuanbaomall.cn

[R01] shebang 与严格模式
来源：http://ijo.yuxming.cn

#!/usr/bin/env bash
来源：http://njb.xingfuxueyuan.xyz

set -euo pipefail
来源：http://oyt.bbcook.cn

[R02] 变量赋值与使用
来源：http://jlg.shanyushiyangtech.top

name="Tom"; echo "$name"
来源：http://pej.fengsongda.top

[R03] 只读变量
来源：http://ygt.yj20258888.top

readonly PI=3.14
来源：http://tbl.hcnkem.com

[R04] 位置参数
来源：http://mfx.tarul.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://azt.bjfxy.top

[R05] 参数默认值
来源：http://vds.tanke756.top

name="${1:-default}"
来源：http://nso.yj20258888.top

[R06] 判断命令是否存在
来源：http://dvr.chenzaomai.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gep.snrcjt.cn

[R07] if 判断文件
来源：http://mev.ydjk.org.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ugp.wangshuangyany.cn

[R08] 数值比较
来源：http://dsy.nwbrower.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zzl.nanxinkj.top

[R09] 字符串比较
来源：http://tdn.shanyushiyangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mnj.quarkkingdee.top

[R10] 正则匹配
来源：http://cxb.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ocj.zhengqikj.top

[R11] case 多分支
来源：http://pox.jinqigfzy.top

case "$1" in
来源：http://mat.tarul.cn

start) echo "启动" ;;
来源：http://jvj.xziqi.cn

stop)  echo "停止" ;;
来源：http://mgg.cqqwz.cn

*)     echo "未知命令" ;;
来源：http://heq.wangshuangyany.cn

esac
来源：http://gcs.iojbl.cn

[R12] for 遍历文件
来源：http://hiw.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://zss.52xcode.cn

[R13] for 计数循环
来源：http://ppv.haohaochexian.top

for i in {1..10}; do echo "$i"; done
来源：http://ble.epnwcf.com

[R14] C 风格 for
来源：http://qzp.ydzc1.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://glb.aizwys.cn

[R15] while 逐行读文件
来源：http://wji.xinyue.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ion.dashuyun.cn

[R16] until 等待条件
来源：http://dra.tianlin.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rby.shzxlz.cn

[R17] 数组定义与取值
来源：http://dsw.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://oym.jiagoushi.top

[R18] 遍历数组
来源：http://oci.jqgufenzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xcz.zhixingplan.top

[R19] 数组长度
来源：http://zye.hnxiangtu.top

echo "${#arr[@]}"
来源：http://frz.fktsv.cn

[R20] 关联数组（字典）
来源：http://vcn.cdnleiting.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pmo.fktsv.cn

[R21] 字符串长度
来源：http://ift.jinqigfzy.top

echo "${#s}"
来源：http://uvs.xuanzx.com

[R22] 截取子串
来源：http://rxc.ybcxt.top

echo "${s:0:5}"
来源：http://tvt.ydzc1.top

[R23] 字符串替换
来源：http://vkx.hnxiangtu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pbu.fanxiaobao.xyz

[R24] 大小写转换
来源：http://jbw.yj20258888.top

echo "${s^^}"; echo "${s,,}"
来源：http://oon.zhiwuduotai.top

[R25] 去后缀 / 去前缀
来源：http://yvu.zhaomingkeji.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://lza.sweek.top

[R26] 命令替换
来源：http://sfz.redwolf501.top

now=$(date +%F); echo "$now"
来源：http://oje.nwbrower.top

[R27] 算术展开
来源：http://qxq.yuanzhike.top

echo $((1 + 2 * 3))
来源：http://bma.feifeiyinyue.top

[R28] 浮点运算
来源：http://bmn.iojbl.cn

echo "scale=2; 10/3" | bc
来源：http://zkd.tianlin.xyz

[R29] 定义函数
来源：http://vtn.shzxlz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zvy.ywan-chungtsiang.top

[R30] 函数返回状态码
来源：http://xif.cdnleiting.top

f() { return 0; }; f || echo "失败了"
来源：http://uap.jqgufenzy.top

[R31] 局部变量
来源：http://hrc.sjlbkw.cn

f() { local x=1; echo "$x"; }
来源：http://tdh.zdqjudy.top

[R32] 参数个数校验
来源：http://axx.pycfn.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hur.jinqigfzy.top

[R33] 捕获错误并提示行号
来源：http://ban.jqgufenzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://inh.redwolf501.top

[R34] 退出时清理
来源：http://oqz.jqgfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://lwn.yanxiufei.cn

[R35] 后台执行并等待
来源：http://ciy.mhx1999.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mfi.jianghu66.top

[R36] 并发执行多个任务
来源：http://fhf.sxryk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ens.52xcode.cn

[R37] 把输出赋给变量
来源：http://zyx.yangfankeji.com

files=$(ls -1)
来源：http://fme.hcnkem.com

[R38] 管道串联
来源：http://zfz.uphjek.com

cat a.txt | grep -i error | wc -l
来源：http://amh.hesvh.cn

[R39] 重定向标准输出与错误
来源：http://neq.cucudq.cn

cmd > out.log 2>&1
来源：http://eeq.redwolf501.top

[R40] 追加写日志
来源：http://qbi.redwolf501.top

echo "log" >> out.log
来源：http://rff.chenzaomai.com

[R41] 丢弃输出
来源：http://nac.yuxming.cn

cmd >/dev/null 2>&1
来源：http://psa.cqqwz.cn

[R42] 输入重定向
来源：http://uuy.ywan-chungtsiang.top

wc -l < a.txt
来源：http://ruk.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://ors.hnqzz.top

find . -name "*.log" -type f
来源：http://lvf.gogol.net.cn

[R44] 按修改时间查找
来源：http://kcc.jinyuanbaomall.cn

find . -mtime -7 -type f
来源：http://pjm.yfazqb.com

[R45] 批量删除
来源：http://mlk.shangyingyoupin.top

find . -name "*.tmp" -delete
来源：http://uyv.meibo888.top

[R46] 递归替换文件内容
来源：http://obe.ivvv.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fzq.yj20258.top

[R47] sed 单行替换
来源：http://mcn.birdmap.top

sed -i 's/foo/bar/g' a.txt
来源：http://spi.ppjwa.cn

[R48] awk 取指定列
来源：http://fke.ppjwa.cn

awk '{print $1, $3}' a.txt
来源：http://vhk.quarkkingdee.top

[R49] awk 带条件
来源：http://wgt.ywan-chungtsiang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rld.gotoacloud.top

[R50] awk 求和
来源：http://ngj.yj20258888.top

awk '{s += $2} END {print s}' a.txt
来源：http://emh.yj202588.top

[R51] 排序去重取前几
来源：http://pyl.hnxiangtu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://uch.cucudq.cn

[R52] 统计行数
来源：http://dkz.yj20258888.top

wc -l a.txt
来源：http://gwr.ppjwa.cn

[R53] 查看文件头与实时尾
来源：http://bzj.wangshuangyany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qtg.birdmap.top

[R54] 比较两个文件
来源：http://whx.ywan-chungtsiang.top

diff a.txt b.txt
来源：http://wef.zhixingplan.top

[R55] 压缩与解压
来源：http://qzr.hnqzz.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jql.xziqi.cn

[R56] 远程拷贝
来源：http://jvi.xylfe.cn

scp file user@host:/path/
来源：http://qbn.chenzaomai.com

[R57] 远程执行命令
来源：http://rbw.aibaodan.cn

ssh user@host 'uptime'
来源：http://jup.yongpay.top

[R58] 下载文件
来源：http://wpk.yj20258.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zzo.xingfuxueyuan.xyz

[R59] 发 POST JSON
来源：http://qhp.hnqzz.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vbb.zdbjq.cn

[R60] 只看 HTTP 状态码
来源：http://bpv.sufxvd.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kva.yj20258.top

[R61] 磁盘占用
来源：http://dez.hnqzz.top

df -h;  du -sh *
来源：http://qoq.wangdashe.top

[R62] 找最占空间的文件
来源：http://hnz.meibo888.top

du -ah . | sort -rh | head -10
来源：http://llp.316326.xyz

[R63] 内存与进程
来源：http://bdr.tian-w.cn

free -h;  ps aux | grep nginx
来源：http://iwc.fehbvm.com

[R64] 结束进程
来源：http://phy.cheryme.top

kill -9 $(pgrep -f app.py)
来源：http://csr.sufxvd.cn

[R65] 查看端口占用
来源：http://wef.zdbjq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://amt.chenjidiqi.icu

[R66] 定时任务
来源：http://new.shanyushiyangtech.top

crontab -e;  crontab -l
来源：http://kfj.cqqwz.cn

[R67] 生成随机十六进制串
来源：http://mga.andypj.xyz

openssl rand -hex 16
来源：http://mqk.yongpay.top

[R68] 计算文件校验值
来源：http://euf.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://dna.feifeiyinyue.top

[R69] 生成随机密码
来源：http://oda.wangshuangyany.cn

head -c 16 /dev/urandom | base64
来源：http://xgc.uphjek.com

[R70] 时间戳与互转
来源：http://jtw.hnqzz.top

date +%s;  date -d @1700000000
来源：http://jbt.aibaodan.cn

[R71] 日期格式化
来源：http://rlf.cucudq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ypo.zycfv.cn

[R72] 等待端口就绪
来源：http://aat.tianlin.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://kxe.xingfuxueyuan.xyz

[R73] 分割大日志
来源：http://zel.316326.xyz

split -l 1000 big.log part_
来源：http://xjg.chenzaomai.com

[R74] 批量重命名
来源：http://ion.ydzc1.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dpv.jyoumei.cn

[R75] 导出环境变量
来源：http://ycq.yfazqb.com

export PATH="$HOME/bin:$PATH"
来源：http://fut.aibaodan.cn

[R76] 使用临时文件
来源：http://fxv.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rxs.ybcxt.top

[R77] 读取用户输入
来源：http://ddk.sjlbkw.cn

read -rp "请输入: " ans
来源：http://kby.ybcxt.top

[R78] 交互式菜单
来源：http://mny.zhixingplan.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tqx.cdnleiting.top

[R79] 解析命令行选项
来源：http://gvl.jinqigfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://opd.hywenlv.cn

[R80] 查看脚本执行耗时
来源：http://qsw.nanxuanxn.top

time ./run.sh
来源：http://eub.vqdsnc.cn

================================================================================
来源：http://bdw.jyoumei.cn

S. C / C++ 专题
来源：http://hft.daxiang520.top

================================================================================
来源：http://rfl.quarkkingdee.top

[S01] C：Hello World
来源：http://yyk.nwbrower.top

#include <stdio.h>
来源：http://hec.yongpay.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zxv.ywan-chungtsiang.top

[S02] C：变量与格式化输出
来源：http://ffm.yangfankeji.com

int a = 10; printf("%d\n", a);
来源：http://znk.sysykeji.top

[S03] C：读入整数
来源：http://ggz.hcnkem.com

int x; scanf("%d", &x);
来源：http://yxc.jianghu66.top

[S04] C：字符串复制
来源：http://wix.pengpengdd.cyou

char dst[32]; strcpy(dst, "hi");
来源：http://hrd.fehbvm.com

[S05] C：字符串长度
来源：http://owm.feifeiyinyue.top

strlen(s)
来源：http://ukw.0kj1m.cn

[S06] C：字符串比较
来源：http://stx.aizwys.cn

strcmp(a, b) == 0
来源：http://ols.zhaomingkeji.xyz

[S07] C：数组遍历求和
来源：http://mul.yanxiufei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mdc.chenlongwang.top

[S08] C：动态内存分配与释放
来源：http://cnk.smart0.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qqy.sxryk.cn

[S09] C：结构体定义与初始化
来源：http://fcm.hysaishi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aag.daria6918.cn

[S10] C：指针与解引用
来源：http://nie.jianghu66.top

int *p = &a;  *p = 5;
来源：http://oje.jqgfzy.top

[S11] C：逐行读文件
来源：http://hrj.ehwqpu.com

FILE *f = fopen("a.txt", "r");
来源：http://ori.epnwcf.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://jhm.ywan-chungtsiang.top

fclose(f);
来源：http://gpv.shangyingyoupin.top

[S12] C：写文件
来源：http://xgv.zycfv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://snk.bbcook.cn

[S13] C：宏定义
来源：http://nxt.tianlin.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hye.gotoacloud.top

[S14] C：枚举
来源：http://zpn.zhijiandao.cn

enum Color { RED, GREEN, BLUE };
来源：http://cnf.ybcxt.top

[S15] C：类型转换
来源：http://ouk.ywan-chungtsiang.top

(double) a / b
来源：http://cmi.yj20258.top

[S16] C：位操作置位
来源：http://bbe.yuanzhike.top

x |= (1 << 3);
来源：http://swc.ehwqpu.com

[S17] C：安全拼接字符串
来源：http://tqs.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xhk.chenzaomai.com

[S18] C：命令行参数
来源：http://bbf.jinyuanbaomall.cn

int main(int argc, char **argv)
来源：http://gsl.hnqzz.top

[S19] C：快速排序
来源：http://bie.smart0.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://yst.chenlongwang.top

[S20] C：二分查找
来源：http://rmt.chenzaomai.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vpu.dianchejie.cn

[S21] C：字符类别判断
来源：http://opa.shzxlz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://syi.sweek.top

[S22] C：字符串转数字
来源：http://vgi.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kez.meibo888.top

[S23] C：随机数
来源：http://dwl.zhoulong.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://jtb.yongpay.top

[S24] C：获取本地时间
来源：http://pnf.jianghu66.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lhv.9152youxi.cn

[S25] C：内存拷贝
来源：http://mgv.svipenyu.cn

memcpy(dst, src, n);
来源：http://aof.ywan-chungtsiang.top

[S26] C：内存清零
来源：http://oyw.wangshuangyany.cn

memset(a, 0, sizeof a);
来源：http://jvh.sufxvd.cn

[S27] C：定义常量
来源：http://rmg.snrcjt.cn

const double PI = 3.14159;
来源：http://yxl.yj202588.top

[S28] C：静态变量
来源：http://app.cheryme.top

static int counter = 0;
来源：http://iuc.xingfuxueyuan.xyz

[S29] C：变参函数
来源：http://dth.tian-w.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oii.ywan-chungtsiang.top

[S30] C：头文件保护
来源：http://kai.0kj1m.cn

#ifndef X_H
来源：http://yrt.gogol.net.cn

#define X_H
来源：http://zqb.fengsongda.top

#endif
来源：http://ffv.yfazqb.com

[S31] C++：Hello World
来源：http://ori.pycfn.com

#include <iostream>
来源：http://hdd.smart0.xyz

int main() { std::cout << "Hello\n"; }
来源：http://dvy.gotoacloud.top

[S32] C++：字符串
来源：http://inx.9152youxi.cn

std::string s = "hi";  s += "!";
来源：http://brm.uphjek.com

[S33] C++：vector 增删
来源：http://mqz.hywenlv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yrb.shanyushiyangkeji.top

[S34] C++：遍历 vector
来源：http://hus.cashguo.top

for (auto &x : v) { std::cout << x; }
来源：http://pji.yangfankeji.com

[S35] C++：map
来源：http://lss.chenlongwang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xqb.haohaochexian.top

[S36] C++：unordered_map
来源：http://wui.yonumen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kge.xingfuxueyuan.xyz

[S37] C++：set
来源：http://qjk.jinqigufen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kuq.cqqwz.cn

[S38] C++：排序
来源：http://aef.hammf.cn

std::sort(v.begin(), v.end());
来源：http://kns.c1oappe.top

[S39] C++：自定义比较器排序
来源：http://qww.52xcode.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eae.tanke756.top

[S40] C++：查找元素
来源：http://tqg.shuidangran.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ozl.aizwys.cn


<!-- 参考信息 -->