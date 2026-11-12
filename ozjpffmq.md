代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wkz.yj20258888.top

[Q58] 累计求和
来源：http://mry.yvedp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ikd.pycfn.com

[Q59] 分组内累计
来源：http://riz.cqqwz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://agc.ywan-chungtsiang.top

[Q60] 取上一行 / 下一行
来源：http://kqm.kuanghao11.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xsp.zdqjudy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yur.guannengcc.top

[Q61] 移动平均
来源：http://que.xuetiantiany.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pui.guowangkeji.top

[Q62] 分组占比
来源：http://nzb.jiagoushi.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ntr.dashuyun.cn

[Q63] 开启事务
来源：http://adb.chenlongwang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ngx.wangdashe.top

[Q64] 提交事务
来源：http://nwy.nanxuanxn.top

COMMIT;
来源：http://jqo.wangdashe.top

[Q65] 回滚事务
来源：http://zpc.yuxming.cn

ROLLBACK;
来源：http://kup.ivvv.top

[Q66] 行锁查询
来源：http://ncm.xziqi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vka.feifeiyinyue.top

[Q67] 设置隔离级别
来源：http://tzg.wangdashe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yph.ppjwa.cn

[Q68] 保存点
来源：http://snn.yuxming.cn

SAVEPOINT sp1;
来源：http://eps.c1oappe.top

ROLLBACK TO sp1;
来源：http://cqx.dashuyun.cn

[Q69] 查看执行计划
来源：http://hzm.mhx1999.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://evt.fengsongda.top

[Q70] 更新统计信息
来源：http://fsp.zhiwuduotai.top

ANALYZE TABLE users;
来源：http://yak.fengsongda.top

[Q71] 查看建表语句
来源：http://qvt.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cjd.sufxvd.cn

[Q72] 查看索引
来源：http://gys.tian-w.cn

SHOW INDEX FROM users;
来源：http://biv.fengsongda.top

[Q73] 查看表状态
来源：http://lse.nwbrower.top

SHOW TABLE STATUS LIKE 'users';
来源：http://adb.quarkkingdee.top

[Q74] 强制使用索引
来源：http://iwb.vehdjk.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uwd.haohaochexian.top

[Q75] 日期格式化
来源：http://mpc.birdmap.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rqm.ctjpmb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cjw.chenzaomai.com

[Q76] 按天统计
来源：http://shg.316326.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rja.zhijiandao.cn

[Q77] 时间加减
来源：http://jrx.daxiang520.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hvn.0kj1m.cn

[Q78] 当前时间
来源：http://hgl.hongshengwenyu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dvh.sysykeji.top

[Q79] 字符串拼接
来源：http://wlo.jinqigufen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hjc.jinqigfzy.top

[Q80] 字符串截取
来源：http://snp.ivvv.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sac.ctjpmb.com

[Q81] 字符串替换
来源：http://hsc.mhx1999.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qrf.haohaochexian.top

[Q82] 字符长度与字节长度
来源：http://nyo.jinqigfzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wpp.ydjk.org.cn

[Q83] 大小写转换
来源：http://rti.zhaomingkeji.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://znc.9152youxi.cn

[Q84] 去除首尾空格
来源：http://fui.yuxming.cn

SELECT TRIM(name) FROM users;
来源：http://lak.jinyuanbaomall.cn

[Q85] 数值取整
来源：http://dni.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yuu.shuidangran.top

[Q86] 读取 JSON 字段
来源：http://grw.yvedp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vss.yj20258888.top

[Q87] JSON 字段做条件
来源：http://evn.dashuyun.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qyj.vqdsnc.cn

[Q88] 行转列（条件聚合）
来源：http://ppr.smart0.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dpr.52xcode.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tij.zhixingplan.top

[Q89] 判断表是否存在
来源：http://otf.yj20258.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yki.redwolf501.top

[Q90] 生成序号列
来源：http://ybz.redwolf501.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lya.yangfankeji.com

================================================================================
来源：http://iwh.ctjpmb.com

R. Bash 专题
来源：http://xdw.guowangkeji.top

================================================================================
来源：http://ozj.iojbl.cn

[R01] shebang 与严格模式
来源：http://hlg.yangfankeji.com

#!/usr/bin/env bash
来源：http://bho.zdqjudy.top

set -euo pipefail
来源：http://edq.zhaomingkeji.xyz

[R02] 变量赋值与使用
来源：http://zme.xingfuxueyuan.xyz

name="Tom"; echo "$name"
来源：http://bxb.yongpay.top

[R03] 只读变量
来源：http://dmt.fktsv.cn

readonly PI=3.14
来源：http://oed.iojbl.cn

[R04] 位置参数
来源：http://ums.zhongyouzk.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ptx.wangshuangyany.cn

[R05] 参数默认值
来源：http://zgy.xuetiantiany.cn

name="${1:-default}"
来源：http://vft.daria6918.cn

[R06] 判断命令是否存在
来源：http://mmt.tarul.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rle.yfazqb.com

[R07] if 判断文件
来源：http://igs.vqdsnc.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hbd.chenjidiqi.icu

[R08] 数值比较
来源：http://emd.iojbl.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dvw.chenlongwang.top

[R09] 字符串比较
来源：http://hbl.jinyuanbaomall.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yof.shzxlz.cn

[R10] 正则匹配
来源：http://dag.jinqigufen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xcj.iojbl.cn

[R11] case 多分支
来源：http://ght.birdmap.top

case "$1" in
来源：http://wmt.yangfankeji.com

start) echo "启动" ;;
来源：http://epa.uphjek.com

stop)  echo "停止" ;;
来源：http://nzx.haohaochexian.top

*)     echo "未知命令" ;;
来源：http://qej.dashuyun.cn

esac
来源：http://oqr.316326.xyz

[R12] for 遍历文件
来源：http://yga.shangyingyoupin.top

for f in *.txt; do echo "$f"; done
来源：http://qbs.mhx1999.top

[R13] for 计数循环
来源：http://vct.chenjidiqi.icu

for i in {1..10}; do echo "$i"; done
来源：http://ypo.fktsv.cn

[R14] C 风格 for
来源：http://vuy.yj202588.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tux.xingfuxueyuan.xyz

[R15] while 逐行读文件
来源：http://ojf.fehbvm.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bxn.dashuyun.cn

[R16] until 等待条件
来源：http://les.daria6918.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fuz.zhixingplan.top

[R17] 数组定义与取值
来源：http://khu.fanxiaobao.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://jbb.sxryk.cn

[R18] 遍历数组
来源：http://rdz.zdqjudy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tui.aizwys.cn

[R19] 数组长度
来源：http://irs.tian-w.cn

echo "${#arr[@]}"
来源：http://nmx.snrcjt.cn

[R20] 关联数组（字典）
来源：http://gzl.ydjk.org.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yvk.zdbjq.cn

[R21] 字符串长度
来源：http://mim.guannengcc.top

echo "${#s}"
来源：http://ckd.haohaochexian.top

[R22] 截取子串
来源：http://nln.jinghuilouyu.cn

echo "${s:0:5}"
来源：http://lfk.vehdjk.com

[R23] 字符串替换
来源：http://bmq.bjfxy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://juv.52xcode.cn

[R24] 大小写转换
来源：http://rxu.feifeiyinyue.top

echo "${s^^}"; echo "${s,,}"
来源：http://ovc.shuidangran.top

[R25] 去后缀 / 去前缀
来源：http://abc.aizwys.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zut.vehdjk.com

[R26] 命令替换
来源：http://jga.iojbl.cn

now=$(date +%F); echo "$now"
来源：http://kwb.cqqwz.cn

[R27] 算术展开
来源：http://fbl.fehbvm.com

echo $((1 + 2 * 3))
来源：http://tpq.vqdsnc.cn

[R28] 浮点运算
来源：http://pda.haohaochexian.top

echo "scale=2; 10/3" | bc
来源：http://pfg.nwbrower.top

[R29] 定义函数
来源：http://qml.cashguo.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xme.sjlbkw.cn

[R30] 函数返回状态码
来源：http://wnp.ehwqpu.com

f() { return 0; }; f || echo "失败了"
来源：http://axu.sysykeji.top

[R31] 局部变量
来源：http://nit.hnxiangtu.top

f() { local x=1; echo "$x"; }
来源：http://qgu.cucudq.cn

[R32] 参数个数校验
来源：http://vaz.zhiwuduotai.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hpo.pengpengdd.cyou

[R33] 捕获错误并提示行号
来源：http://brk.yonumen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xyl.sjlbkw.cn

[R34] 退出时清理
来源：http://zgy.fehbvm.com

trap 'rm -f "$tmp"' EXIT
来源：http://bqh.gotoacloud.top

[R35] 后台执行并等待
来源：http://puu.ctjpmb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://ftr.birdmap.top

[R36] 并发执行多个任务
来源：http://ybv.zhiwuduotai.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://itp.daxiang520.top

[R37] 把输出赋给变量
来源：http://bin.xinyue.icu

files=$(ls -1)
来源：http://fsx.nanxinkj.top

[R38] 管道串联
来源：http://qop.svipenyu.cn

cat a.txt | grep -i error | wc -l
来源：http://aol.yvedp.cn

[R39] 重定向标准输出与错误
来源：http://vvb.shanyushiyangtech.top

cmd > out.log 2>&1
来源：http://hem.wangshuangyany.cn

[R40] 追加写日志
来源：http://unf.yanxiufei.cn

echo "log" >> out.log
来源：http://hwk.hysaishi.cn

[R41] 丢弃输出
来源：http://rub.aizwys.cn

cmd >/dev/null 2>&1
来源：http://baz.jinghuilouyu.cn

[R42] 输入重定向
来源：http://yiq.hywenlv.cn

wc -l < a.txt
来源：http://blh.shangyingyoupin.top

[R43] 按名字查找文件
来源：http://pjc.aizwys.cn

find . -name "*.log" -type f
来源：http://wyw.tanke756.top

[R44] 按修改时间查找
来源：http://koz.meibo888.top

find . -mtime -7 -type f
来源：http://nds.cqqwz.cn

[R45] 批量删除
来源：http://gxy.yueranfly.top

find . -name "*.tmp" -delete
来源：http://hkc.hnqzz.top

[R46] 递归替换文件内容
来源：http://uwl.cucudq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ike.kuanghao11.cn

[R47] sed 单行替换
来源：http://hnm.hnqzz.top

sed -i 's/foo/bar/g' a.txt
来源：http://rtq.bbcook.cn

[R48] awk 取指定列
来源：http://olj.zhixingplan.top

awk '{print $1, $3}' a.txt
来源：http://dbk.jlsjyb.cn

[R49] awk 带条件
来源：http://mxg.fktsv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rtx.kuanghao11.cn

[R50] awk 求和
来源：http://ahv.hnxiangtu.top

awk '{s += $2} END {print s}' a.txt
来源：http://hxn.ywan-chungtsiang.top

[R51] 排序去重取前几
来源：http://gnn.zhongyouzk.top

sort a.txt | uniq -c | sort -rn | head
来源：http://wdc.zhijiandao.cn

[R52] 统计行数
来源：http://klg.hnqzz.top

wc -l a.txt
来源：http://hju.xinyue.icu

[R53] 查看文件头与实时尾
来源：http://zwy.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nur.shanyushiyangtech.top

[R54] 比较两个文件
来源：http://vmz.cucudq.cn

diff a.txt b.txt
来源：http://dzu.fehbvm.com

[R55] 压缩与解压
来源：http://gqx.nanxinkj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xff.ywan-chungtsiang.top

[R56] 远程拷贝
来源：http://con.yvedp.cn

scp file user@host:/path/
来源：http://voy.bbcook.cn

[R57] 远程执行命令
来源：http://rla.xuetiantiany.cn

ssh user@host 'uptime'
来源：http://xhu.gotoacloud.top

[R58] 下载文件
来源：http://ljs.hcnkem.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xlo.zhiwuduotai.top

[R59] 发 POST JSON
来源：http://ciz.nwbrower.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gbe.zhixingplan.top

[R60] 只看 HTTP 状态码
来源：http://ymk.jqgfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kps.fehbvm.com

[R61] 磁盘占用
来源：http://ytc.jlsjyb.cn

df -h;  du -sh *
来源：http://zhd.epnwcf.com

[R62] 找最占空间的文件
来源：http://bvy.zhiwuduotai.top

du -ah . | sort -rh | head -10
来源：http://nni.jqgfzy.top

[R63] 内存与进程
来源：http://xnb.smart0.xyz

free -h;  ps aux | grep nginx
来源：http://zdc.vqdsnc.cn

[R64] 结束进程
来源：http://yml.zhaomingkeji.xyz

kill -9 $(pgrep -f app.py)
来源：http://ubi.dianchejie.cn

[R65] 查看端口占用
来源：http://xfd.jlsjyb.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cyx.shzxlz.cn

[R66] 定时任务
来源：http://nhy.epnwcf.com

crontab -e;  crontab -l
来源：http://ibj.xylfe.cn

[R67] 生成随机十六进制串
来源：http://uzg.jqgfzy.top

openssl rand -hex 16
来源：http://hkj.tianlin.xyz

[R68] 计算文件校验值
来源：http://fbz.havefunace.top

sha256sum a.txt;  md5sum a.txt
来源：http://ckx.yvedp.cn

[R69] 生成随机密码
来源：http://rjq.jiagoushi.top

head -c 16 /dev/urandom | base64
来源：http://uwn.ctjpmb.com

[R70] 时间戳与互转
来源：http://hqi.nanxinkj.top

date +%s;  date -d @1700000000
来源：http://lpm.jqgufenzy.top

[R71] 日期格式化
来源：http://zct.shanyushiyangtech.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://avq.xingfuxueyuan.xyz

[R72] 等待端口就绪
来源：http://ljv.wangshuangyany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lxv.mhx1999.top

[R73] 分割大日志
来源：http://rje.yonumen.top

split -l 1000 big.log part_
来源：http://nkd.nanxinkj.top

[R74] 批量重命名
来源：http://ecj.daria6918.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jiw.nwbrower.top

[R75] 导出环境变量
来源：http://jnb.tianlin.xyz

export PATH="$HOME/bin:$PATH"
来源：http://hod.shuidangran.top

[R76] 使用临时文件
来源：http://rrk.jinqigufen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hwi.nanxuanxn.top

[R77] 读取用户输入
来源：http://uww.shanyushiyangtech.top

read -rp "请输入: " ans
来源：http://ynx.tarul.cn

[R78] 交互式菜单
来源：http://ucs.zycfv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gif.shuidangran.top

[R79] 解析命令行选项
来源：http://gcc.nanxuanxn.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rya.pengpengdd.cyou

[R80] 查看脚本执行耗时
来源：http://vin.ctjpmb.com

time ./run.sh
来源：http://gux.aizwys.cn

================================================================================
来源：http://fmu.yongpay.top

S. C / C++ 专题
来源：http://rrw.epnwcf.com

================================================================================
来源：http://fxc.gogol.net.cn

[S01] C：Hello World
来源：http://uvr.ybcxt.top

#include <stdio.h>
来源：http://asd.meibo888.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dui.vqdsnc.cn

[S02] C：变量与格式化输出
来源：http://rlx.zhaomingkeji.xyz

int a = 10; printf("%d\n", a);
来源：http://evl.tarul.cn

[S03] C：读入整数
来源：http://ryg.vqdsnc.cn

int x; scanf("%d", &x);
来源：http://iqe.yj202588.top

[S04] C：字符串复制
来源：http://trf.vehdjk.com

char dst[32]; strcpy(dst, "hi");
来源：http://kpj.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://iyz.0kj1m.cn

strlen(s)
来源：http://gvd.nanxuanxn.top

[S06] C：字符串比较
来源：http://qdj.zhiwuduotai.top

strcmp(a, b) == 0
来源：http://btf.yangfankeji.com

[S07] C：数组遍历求和
来源：http://wui.hesvh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rii.jiagoushi.top

[S08] C：动态内存分配与释放
来源：http://fnk.zhoulong.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://svh.yanxiufei.cn

[S09] C：结构体定义与初始化
来源：http://qag.ywan-chungtsiang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ogc.xuanzx.com

[S10] C：指针与解引用
来源：http://zig.cashguo.top

int *p = &a;  *p = 5;
来源：http://upf.pycfn.com

[S11] C：逐行读文件
来源：http://lwd.fehbvm.com

FILE *f = fopen("a.txt", "r");
来源：http://gtz.svipenyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ilv.ctjpmb.com

fclose(f);
来源：http://bxa.kuanghao11.cn

[S12] C：写文件
来源：http://pkf.xylfe.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rml.haohaochexian.top

[S13] C：宏定义
来源：http://icn.chenlongwang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wlt.tanke756.top

[S14] C：枚举
来源：http://kka.aibaodan.cn

enum Color { RED, GREEN, BLUE };
来源：http://vbc.xylfe.cn

[S15] C：类型转换
来源：http://jqb.0kj1m.cn

(double) a / b
来源：http://vqt.tianlin.xyz

[S16] C：位操作置位
来源：http://xpf.fehbvm.com

x |= (1 << 3);
来源：http://lyy.chenlongwang.top

[S17] C：安全拼接字符串
来源：http://yaj.vehdjk.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lqw.jinqigfzy.top

[S18] C：命令行参数
来源：http://edr.cucudq.cn

int main(int argc, char **argv)
来源：http://imh.vqdsnc.cn

[S19] C：快速排序
来源：http://uxw.havefunace.top

qsort(a, n, sizeof(int), cmp);
来源：http://iyh.fzhhl.top

[S20] C：二分查找
来源：http://ura.redwolf501.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fgi.nwbrower.top

[S21] C：字符类别判断
来源：http://kcv.nanxuanxn.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ijs.tarul.cn

[S22] C：字符串转数字
来源：http://pwl.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mud.sjlbkw.cn

[S23] C：随机数
来源：http://uuu.aibaodan.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://edu.ehwqpu.com

[S24] C：获取本地时间
来源：http://uxs.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gpp.daxiang520.top

[S25] C：内存拷贝
来源：http://hfb.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://goo.gogol.net.cn

[S26] C：内存清零
来源：http://mzd.wangshuangyany.cn

memset(a, 0, sizeof a);
来源：http://mvh.fehbvm.com

[S27] C：定义常量
来源：http://ynw.jianghu66.top

const double PI = 3.14159;
来源：http://udi.316326.xyz

[S28] C：静态变量
来源：http://fqb.ehwqpu.com


<!-- 参考信息 -->