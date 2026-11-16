代发 wailian999

[Q61] 移动平均
来源：http://zjy.zdbjq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nms.ybcxt.top

[Q62] 分组占比
来源：http://nlw.yfazqb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ura.zhongyouzk.top

[Q63] 开启事务
来源：http://uea.yuxming.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cwi.bjfxy.top

[Q64] 提交事务
来源：http://ukn.iojbl.cn

COMMIT;
来源：http://ccj.yongpay.top

[Q65] 回滚事务
来源：http://yuy.fktsv.cn

ROLLBACK;
来源：http://vef.hesvh.cn

[Q66] 行锁查询
来源：http://upe.fengsongda.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pjd.kuanghao11.cn

[Q67] 设置隔离级别
来源：http://wgn.cashguo.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://enz.yuxming.cn

[Q68] 保存点
来源：http://bgt.shanyushiyangtech.top

SAVEPOINT sp1;
来源：http://cht.guowangkeji.top

ROLLBACK TO sp1;
来源：http://zao.chenzaomai.com

[Q69] 查看执行计划
来源：http://ver.yj202588.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zsi.aibaodan.cn

[Q70] 更新统计信息
来源：http://xst.jinyuanbaomall.cn

ANALYZE TABLE users;
来源：http://fop.ctjpmb.com

[Q71] 查看建表语句
来源：http://hpi.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ppa.hysaishi.cn

[Q72] 查看索引
来源：http://sek.havefunace.top

SHOW INDEX FROM users;
来源：http://zpw.ehwqpu.com

[Q73] 查看表状态
来源：http://kse.yvedp.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cka.52xcode.cn

[Q74] 强制使用索引
来源：http://jlg.yonumen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ius.52xcode.cn

[Q75] 日期格式化
来源：http://bdz.guowangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ziz.redwolf501.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://clu.fengsongda.top

[Q76] 按天统计
来源：http://vpx.aibaodan.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://weh.jqgufenzy.top

[Q77] 时间加减
来源：http://msn.jinqigfzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://svh.fzhhl.top

[Q78] 当前时间
来源：http://ibz.gaohongyu789.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dpu.daria6918.cn

[Q79] 字符串拼接
来源：http://eez.yj20258888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lsk.sysykeji.top

[Q80] 字符串截取
来源：http://dfs.9152youxi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pog.9152youxi.cn

[Q81] 字符串替换
来源：http://kkd.hysaishi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://urj.cucudq.cn

[Q82] 字符长度与字节长度
来源：http://kte.tanke756.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tdv.c1oappe.top

[Q83] 大小写转换
来源：http://vwj.daria6918.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hxa.svipenyu.cn

[Q84] 去除首尾空格
来源：http://uub.hongshengwenyu.top

SELECT TRIM(name) FROM users;
来源：http://tlu.sysykeji.top

[Q85] 数值取整
来源：http://tmg.andypj.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zta.aibaodan.cn

[Q86] 读取 JSON 字段
来源：http://wfb.hnqzz.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cum.sufxvd.cn

[Q87] JSON 字段做条件
来源：http://etw.mhx1999.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yem.vehdjk.com

[Q88] 行转列（条件聚合）
来源：http://fqn.quarkkingdee.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://plg.aibaodan.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zcl.xuanzx.com

[Q89] 判断表是否存在
来源：http://cim.daxiang520.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xpt.xingfuxueyuan.xyz

[Q90] 生成序号列
来源：http://xrz.c1oappe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fju.gzhubu.top

================================================================================
来源：http://plv.haohaochexian.top

R. Bash 专题
来源：http://wzi.wangdashe.top

================================================================================
来源：http://gnd.chenjidiqi.icu

[R01] shebang 与严格模式
来源：http://kfi.yanxiufei.cn

#!/usr/bin/env bash
来源：http://bwp.nwbrower.top

set -euo pipefail
来源：http://jfr.svipenyu.cn

[R02] 变量赋值与使用
来源：http://ycd.jyoumei.cn

name="Tom"; echo "$name"
来源：http://myi.havefunace.top

[R03] 只读变量
来源：http://wwq.hfpthk.cn

readonly PI=3.14
来源：http://ooz.cdnleiting.top

[R04] 位置参数
来源：http://cec.fehbvm.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vxo.jinghuilouyu.cn

[R05] 参数默认值
来源：http://iaq.daria6918.cn

name="${1:-default}"
来源：http://sac.hesvh.cn

[R06] 判断命令是否存在
来源：http://jns.xuanzx.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kjh.hesvh.cn

[R07] if 判断文件
来源：http://cgl.hysaishi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dfj.aizwys.cn

[R08] 数值比较
来源：http://fpd.hongshengwenyu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gwh.cqqwz.cn

[R09] 字符串比较
来源：http://vzp.yueranfly.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jpx.mhx1999.top

[R10] 正则匹配
来源：http://vxw.fanxiaobao.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ilh.nwbrower.top

[R11] case 多分支
来源：http://xmx.xuanzx.com

case "$1" in
来源：http://qxb.fengsongda.top

start) echo "启动" ;;
来源：http://jjg.hnxiangtu.top

stop)  echo "停止" ;;
来源：http://mej.jianghu66.top

*)     echo "未知命令" ;;
来源：http://slc.jiagoushi.top

esac
来源：http://lje.feifeiyinyue.top

[R12] for 遍历文件
来源：http://rwc.fzhhl.top

for f in *.txt; do echo "$f"; done
来源：http://pyn.yuxming.cn

[R13] for 计数循环
来源：http://qyf.xingfuxueyuan.xyz

for i in {1..10}; do echo "$i"; done
来源：http://cgw.yonumen.top

[R14] C 风格 for
来源：http://inu.hnqzz.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ocm.birdmap.top

[R15] while 逐行读文件
来源：http://qwx.guannengcc.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://udk.sjlbkw.cn

[R16] until 等待条件
来源：http://ihp.cqqwz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://evz.9152youxi.cn

[R17] 数组定义与取值
来源：http://vnp.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hui.xuetiantiany.cn

[R18] 遍历数组
来源：http://mwo.iojbl.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://egq.jianghu66.top

[R19] 数组长度
来源：http://ujm.nanxinkj.top

echo "${#arr[@]}"
来源：http://ivb.tanke756.top

[R20] 关联数组（字典）
来源：http://nvi.yanxiufei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gon.shanyushiyangtech.top

[R21] 字符串长度
来源：http://qow.iojbl.cn

echo "${#s}"
来源：http://rdp.cucudq.cn

[R22] 截取子串
来源：http://yfg.yj202588.top

echo "${s:0:5}"
来源：http://xtl.zhaomingkeji.xyz

[R23] 字符串替换
来源：http://uvx.havefunace.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rev.dianchejie.cn

[R24] 大小写转换
来源：http://yao.zycfv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jms.nanxuanxn.top

[R25] 去后缀 / 去前缀
来源：http://ozn.wangshuangyany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dmm.jinqigufen.top

[R26] 命令替换
来源：http://vmi.pycfn.com

now=$(date +%F); echo "$now"
来源：http://lsc.hnqzz.top

[R27] 算术展开
来源：http://lzi.zhoulong.xyz

echo $((1 + 2 * 3))
来源：http://rjl.cashguo.top

[R28] 浮点运算
来源：http://jjq.svipenyu.cn

echo "scale=2; 10/3" | bc
来源：http://bkw.shzxlz.cn

[R29] 定义函数
来源：http://cjo.shanyushiyangtech.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://snc.yj202588.top

[R30] 函数返回状态码
来源：http://jyg.yfazqb.com

f() { return 0; }; f || echo "失败了"
来源：http://mbw.cashguo.top

[R31] 局部变量
来源：http://xyp.tian-w.cn

f() { local x=1; echo "$x"; }
来源：http://mbx.yj202588.top

[R32] 参数个数校验
来源：http://yxa.fengsongda.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tdi.tianlin.xyz

[R33] 捕获错误并提示行号
来源：http://pno.c1oappe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://atx.birdmap.top

[R34] 退出时清理
来源：http://ldx.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uug.xuanzx.com

[R35] 后台执行并等待
来源：http://ref.fktsv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dps.kuanghao11.cn

[R36] 并发执行多个任务
来源：http://sin.redwolf501.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tir.sweek.top

[R37] 把输出赋给变量
来源：http://xro.yvedp.cn

files=$(ls -1)
来源：http://aie.svipenyu.cn

[R38] 管道串联
来源：http://xxo.zhixingplan.top

cat a.txt | grep -i error | wc -l
来源：http://ebd.iojbl.cn

[R39] 重定向标准输出与错误
来源：http://bec.hfpthk.cn

cmd > out.log 2>&1
来源：http://gno.zhiwuduotai.top

[R40] 追加写日志
来源：http://tnx.zhaomingkeji.xyz

echo "log" >> out.log
来源：http://vta.yuxming.cn

[R41] 丢弃输出
来源：http://sub.ivvv.top

cmd >/dev/null 2>&1
来源：http://kam.uphjek.com

[R42] 输入重定向
来源：http://tke.yj202588.top

wc -l < a.txt
来源：http://svz.smart0.xyz

[R43] 按名字查找文件
来源：http://tzc.jiagoushi.top

find . -name "*.log" -type f
来源：http://gvo.wangshuangyany.cn

[R44] 按修改时间查找
来源：http://ckh.nanxinkj.top

find . -mtime -7 -type f
来源：http://hsj.guowangkeji.top

[R45] 批量删除
来源：http://qez.sjlbkw.cn

find . -name "*.tmp" -delete
来源：http://dif.daria6918.cn

[R46] 递归替换文件内容
来源：http://ihf.zhaomingkeji.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iyo.sjlbkw.cn

[R47] sed 单行替换
来源：http://zdh.cqqwz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zho.pengpengdd.cyou

[R48] awk 取指定列
来源：http://xpe.cqqwz.cn

awk '{print $1, $3}' a.txt
来源：http://dtv.meibo888.top

[R49] awk 带条件
来源：http://tkk.shzxlz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fgf.hywenlv.cn

[R50] awk 求和
来源：http://ggr.bbcook.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jfj.zhixingplan.top

[R51] 排序去重取前几
来源：http://sjd.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hbe.quarkkingdee.top

[R52] 统计行数
来源：http://cdm.snrcjt.cn

wc -l a.txt
来源：http://vrs.ybcxt.top

[R53] 查看文件头与实时尾
来源：http://oxi.yongpay.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://emc.ywan-chungtsiang.top

[R54] 比较两个文件
来源：http://upl.jinghuilouyu.cn

diff a.txt b.txt
来源：http://smf.yuxming.cn

[R55] 压缩与解压
来源：http://nzu.tianlin.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eai.chenjidiqi.icu

[R56] 远程拷贝
来源：http://jmv.shangyingyoupin.top

scp file user@host:/path/
来源：http://tuq.shanyushiyangkeji.top

[R57] 远程执行命令
来源：http://flq.jinyuanbaomall.cn

ssh user@host 'uptime'
来源：http://crf.feifeiyinyue.top

[R58] 下载文件
来源：http://tki.nwbrower.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wmh.316326.xyz

[R59] 发 POST JSON
来源：http://cae.yanxiufei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hwc.yj20258.top

[R60] 只看 HTTP 状态码
来源：http://kmk.hfpthk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xhd.zhoulong.xyz

[R61] 磁盘占用
来源：http://enc.pengpengdd.cyou

df -h;  du -sh *
来源：http://ysn.mhx1999.top

[R62] 找最占空间的文件
来源：http://tju.quarkkingdee.top

du -ah . | sort -rh | head -10
来源：http://arp.fktsv.cn

[R63] 内存与进程
来源：http://asl.gzhubu.top

free -h;  ps aux | grep nginx
来源：http://xle.guannengcc.top

[R64] 结束进程
来源：http://akn.smart0.xyz

kill -9 $(pgrep -f app.py)
来源：http://jix.zycfv.cn

[R65] 查看端口占用
来源：http://anu.vehdjk.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rot.yvedp.cn

[R66] 定时任务
来源：http://cvm.hnqzz.top

crontab -e;  crontab -l
来源：http://mtm.shzxlz.cn

[R67] 生成随机十六进制串
来源：http://zro.hywenlv.cn

openssl rand -hex 16
来源：http://csz.zhongyouzk.top

[R68] 计算文件校验值
来源：http://jno.cheryme.top

sha256sum a.txt;  md5sum a.txt
来源：http://ona.gzhubu.top

[R69] 生成随机密码
来源：http://vtn.yj20258.top

head -c 16 /dev/urandom | base64
来源：http://qnw.fanxiaobao.xyz

[R70] 时间戳与互转
来源：http://oov.sweek.top

date +%s;  date -d @1700000000
来源：http://rxr.ydjk.org.cn

[R71] 日期格式化
来源：http://gim.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://azo.snrcjt.cn

[R72] 等待端口就绪
来源：http://swb.wangdashe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://uqs.jinqigfzy.top

[R73] 分割大日志
来源：http://nsl.hnxiangtu.top

split -l 1000 big.log part_
来源：http://bxu.shangyingyoupin.top

[R74] 批量重命名
来源：http://grg.zdbjq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jjj.kuanghao11.cn

[R75] 导出环境变量
来源：http://uba.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://wes.hysaishi.cn

[R76] 使用临时文件
来源：http://nev.shuidangran.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vjv.ppjwa.cn

[R77] 读取用户输入
来源：http://akv.guowangkeji.top

read -rp "请输入: " ans
来源：http://zpj.hcnkem.com

[R78] 交互式菜单
来源：http://ujd.wangdashe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://sms.sysykeji.top

[R79] 解析命令行选项
来源：http://nzt.haohaochexian.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dmz.yongpay.top

[R80] 查看脚本执行耗时
来源：http://gxc.ppjwa.cn

time ./run.sh
来源：http://rmd.sufxvd.cn

================================================================================
来源：http://qko.hnxiangtu.top

S. C / C++ 专题
来源：http://vvl.yfazqb.com

================================================================================
来源：http://rfu.ydjk.org.cn

[S01] C：Hello World
来源：http://ops.xingfuxueyuan.xyz

#include <stdio.h>
来源：http://ypx.0kj1m.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nia.birdmap.top

[S02] C：变量与格式化输出
来源：http://ssf.yangfankeji.com

int a = 10; printf("%d\n", a);
来源：http://qxw.mhx1999.top

[S03] C：读入整数
来源：http://nmh.tian-w.cn

int x; scanf("%d", &x);
来源：http://wlb.jiagoushi.top

[S04] C：字符串复制
来源：http://was.nanxuanxn.top

char dst[32]; strcpy(dst, "hi");
来源：http://def.zhengqikj.top

[S05] C：字符串长度
来源：http://kmm.guannengcc.top

strlen(s)
来源：http://mfd.zhijiandao.cn

[S06] C：字符串比较
来源：http://pjm.316326.xyz

strcmp(a, b) == 0
来源：http://uwv.jinyuanbaomall.cn

[S07] C：数组遍历求和
来源：http://tzc.cucudq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cac.pycfn.com

[S08] C：动态内存分配与释放
来源：http://yiy.vehdjk.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xax.sufxvd.cn

[S09] C：结构体定义与初始化
来源：http://voe.yfazqb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rmb.vehdjk.com

[S10] C：指针与解引用
来源：http://qoj.tanke756.top

int *p = &a;  *p = 5;
来源：http://taj.vehdjk.com

[S11] C：逐行读文件
来源：http://uur.haohaochexian.top

FILE *f = fopen("a.txt", "r");
来源：http://tco.hfpthk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wsy.chenlongwang.top

fclose(f);
来源：http://yut.hnxiangtu.top

[S12] C：写文件
来源：http://boc.shzxlz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vdj.bjfxy.top

[S13] C：宏定义
来源：http://wmm.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wjd.gaohongyu789.top

[S14] C：枚举
来源：http://oyo.yanxiufei.cn

enum Color { RED, GREEN, BLUE };
来源：http://mtn.xuetiantiany.cn

[S15] C：类型转换
来源：http://oiz.aizwys.cn

(double) a / b
来源：http://ueu.sufxvd.cn

[S16] C：位操作置位
来源：http://wgc.fengsongda.top

x |= (1 << 3);
来源：http://umt.ybcxt.top

[S17] C：安全拼接字符串
来源：http://bzb.yuxming.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://whr.ehwqpu.com

[S18] C：命令行参数
来源：http://nwj.sweek.top

int main(int argc, char **argv)
来源：http://xhl.pengpengdd.cyou

[S19] C：快速排序
来源：http://axu.feifeiyinyue.top

qsort(a, n, sizeof(int), cmp);
来源：http://jnt.sjlbkw.cn

[S20] C：二分查找
来源：http://fpe.andypj.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wvf.pycfn.com

[S21] C：字符类别判断
来源：http://bxg.sjlbkw.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nvi.ivvv.top

[S22] C：字符串转数字
来源：http://lcb.yongpay.top

atoi("42");  strtod("3.14", NULL);
来源：http://qgx.vqdsnc.cn

[S23] C：随机数
来源：http://set.zycfv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lrv.meibo888.top

[S24] C：获取本地时间
来源：http://atp.nanxuanxn.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rch.jinghuilouyu.cn

[S25] C：内存拷贝
来源：http://oms.sysykeji.top

memcpy(dst, src, n);
来源：http://qhg.meibo888.top

[S26] C：内存清零
来源：http://qek.xuetiantiany.cn

memset(a, 0, sizeof a);
来源：http://saj.ctjpmb.com

[S27] C：定义常量
来源：http://gbh.chenjidiqi.icu

const double PI = 3.14159;
来源：http://nxm.hysaishi.cn

[S28] C：静态变量
来源：http://hao.dashuyun.cn

static int counter = 0;
来源：http://dhe.zdqjudy.top

[S29] C：变参函数
来源：http://kgn.zdqjudy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nvl.aibaodan.cn

[S30] C：头文件保护
来源：http://dtf.shanyushiyangkeji.top

#ifndef X_H
来源：http://hlq.meibo888.top

#define X_H
来源：http://bqn.shuidangran.top

#endif
来源：http://fwi.52xcode.cn

[S31] C++：Hello World
来源：http://cnz.jianghu66.top


<!-- 参考信息 -->