代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tur.wangdashe.top

[Q56] 密集排名（并列不占位）
来源：http://ecs.meibo888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://apk.zhoulong.xyz

[Q57] 行号
来源：http://nqb.yvedp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cwd.fzhhl.top

[Q58] 累计求和
来源：http://rrf.dashuyun.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gcp.jiagoushi.top

[Q59] 分组内累计
来源：http://afd.daxiang520.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://imr.yuanzhike.top

[Q60] 取上一行 / 下一行
来源：http://rtf.zycfv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gtj.sweek.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://imn.yvedp.cn

[Q61] 移动平均
来源：http://tbg.xingfuxueyuan.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bgw.pengpengdd.cyou

[Q62] 分组占比
来源：http://qsb.zycfv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jdr.jinyuanbaomall.cn

[Q63] 开启事务
来源：http://uil.jyoumei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bsr.bbcook.cn

[Q64] 提交事务
来源：http://gto.andypj.xyz

COMMIT;
来源：http://wvb.bbcook.cn

[Q65] 回滚事务
来源：http://ega.yuanzhike.top

ROLLBACK;
来源：http://diw.yueranfly.top

[Q66] 行锁查询
来源：http://urq.sysykeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pwu.xinyue.icu

[Q67] 设置隔离级别
来源：http://ozq.tian-w.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ior.zhoulong.xyz

[Q68] 保存点
来源：http://jsd.chenlongwang.top

SAVEPOINT sp1;
来源：http://gso.epnwcf.com

ROLLBACK TO sp1;
来源：http://xut.zhaomingkeji.xyz

[Q69] 查看执行计划
来源：http://dsd.feifeiyinyue.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xch.tanke756.top

[Q70] 更新统计信息
来源：http://ajp.redwolf501.top

ANALYZE TABLE users;
来源：http://vnl.zycfv.cn

[Q71] 查看建表语句
来源：http://xfk.jinyuanbaomall.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mip.jinghuilouyu.cn

[Q72] 查看索引
来源：http://xeu.xuanzx.com

SHOW INDEX FROM users;
来源：http://yyy.jyoumei.cn

[Q73] 查看表状态
来源：http://yfm.shuidangran.top

SHOW TABLE STATUS LIKE 'users';
来源：http://yny.zhaomingkeji.xyz

[Q74] 强制使用索引
来源：http://grw.shangyingyoupin.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ktm.fanxiaobao.xyz

[Q75] 日期格式化
来源：http://lef.cashguo.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ljg.shanyushiyangtech.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tuu.havefunace.top

[Q76] 按天统计
来源：http://cri.fzhhl.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bbd.yvedp.cn

[Q77] 时间加减
来源：http://hxh.xuanzx.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jsj.ydjk.org.cn

[Q78] 当前时间
来源：http://oja.dianchejie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mhv.chenlongwang.top

[Q79] 字符串拼接
来源：http://dui.guowangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lyi.yuanzhike.top

[Q80] 字符串截取
来源：http://jvw.yanxiufei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://exn.shanyushiyangtech.top

[Q81] 字符串替换
来源：http://bmd.pycfn.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ikj.316326.xyz

[Q82] 字符长度与字节长度
来源：http://doj.haohaochexian.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xkk.hnqzz.top

[Q83] 大小写转换
来源：http://mnp.yongpay.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://juo.yj20258.top

[Q84] 去除首尾空格
来源：http://npp.zhengqikj.top

SELECT TRIM(name) FROM users;
来源：http://mgm.aizwys.cn

[Q85] 数值取整
来源：http://isy.yangfankeji.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kui.bbcook.cn

[Q86] 读取 JSON 字段
来源：http://har.hcnkem.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xhi.52xcode.cn

[Q87] JSON 字段做条件
来源：http://dby.cucudq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://evo.sweek.top

[Q88] 行转列（条件聚合）
来源：http://cqk.andypj.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://krf.jiagoushi.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cxp.daria6918.cn

[Q89] 判断表是否存在
来源：http://szm.wangshuangyany.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sey.fehbvm.com

[Q90] 生成序号列
来源：http://vmz.jinqigfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dmf.yueranfly.top

================================================================================
来源：http://skq.jyoumei.cn

R. Bash 专题
来源：http://wsz.yfazqb.com

================================================================================
来源：http://dyp.yueranfly.top

[R01] shebang 与严格模式
来源：http://ehq.snrcjt.cn

#!/usr/bin/env bash
来源：http://apu.ydzc1.top

set -euo pipefail
来源：http://mur.gotoacloud.top

[R02] 变量赋值与使用
来源：http://uhj.birdmap.top

name="Tom"; echo "$name"
来源：http://luw.cheryme.top

[R03] 只读变量
来源：http://zba.ehwqpu.com

readonly PI=3.14
来源：http://vqv.cucudq.cn

[R04] 位置参数
来源：http://mhn.havefunace.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://axk.hongshengwenyu.top

[R05] 参数默认值
来源：http://icc.shanyushiyangtech.top

name="${1:-default}"
来源：http://wrj.cashguo.top

[R06] 判断命令是否存在
来源：http://rdy.tian-w.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vul.ybcxt.top

[R07] if 判断文件
来源：http://qxx.cucudq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wjq.uphjek.com

[R08] 数值比较
来源：http://idh.jlsjyb.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://oed.ehwqpu.com

[R09] 字符串比较
来源：http://epz.zycfv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nnj.xinyue.icu

[R10] 正则匹配
来源：http://eyz.smart0.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yip.pycfn.com

[R11] case 多分支
来源：http://ogr.xuanzx.com

case "$1" in
来源：http://jek.52xcode.cn

start) echo "启动" ;;
来源：http://npz.jianghu66.top

stop)  echo "停止" ;;
来源：http://uhq.shzxlz.cn

*)     echo "未知命令" ;;
来源：http://ztf.yangfankeji.com

esac
来源：http://vgp.xuetiantiany.cn

[R12] for 遍历文件
来源：http://fcy.pycfn.com

for f in *.txt; do echo "$f"; done
来源：http://mms.cucudq.cn

[R13] for 计数循环
来源：http://frh.dashuyun.cn

for i in {1..10}; do echo "$i"; done
来源：http://awt.yuanzhike.top

[R14] C 风格 for
来源：http://drm.nanxinkj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wdj.wangshuangyany.cn

[R15] while 逐行读文件
来源：http://aaf.daria6918.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pqg.fktsv.cn

[R16] until 等待条件
来源：http://qfz.xinyue.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rtt.zhoulong.xyz

[R17] 数组定义与取值
来源：http://ege.cheryme.top

arr=(a b c); echo "${arr[0]}"
来源：http://dgv.52xcode.cn

[R18] 遍历数组
来源：http://ena.jlsjyb.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://otv.cheryme.top

[R19] 数组长度
来源：http://uum.hesvh.cn

echo "${#arr[@]}"
来源：http://pti.fengsongda.top

[R20] 关联数组（字典）
来源：http://ehg.quarkkingdee.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zvq.dashuyun.cn

[R21] 字符串长度
来源：http://nam.jiagoushi.top

echo "${#s}"
来源：http://ezd.smart0.xyz

[R22] 截取子串
来源：http://epo.jinyuanbaomall.cn

echo "${s:0:5}"
来源：http://hnk.xylfe.cn

[R23] 字符串替换
来源：http://brd.redwolf501.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xld.shangyingyoupin.top

[R24] 大小写转换
来源：http://kbs.jinqigfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://xeb.sufxvd.cn

[R25] 去后缀 / 去前缀
来源：http://gqh.52xcode.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ihg.ctjpmb.com

[R26] 命令替换
来源：http://fct.jiagoushi.top

now=$(date +%F); echo "$now"
来源：http://etc.zhixingplan.top

[R27] 算术展开
来源：http://hfw.sxryk.cn

echo $((1 + 2 * 3))
来源：http://nzr.shzxlz.cn

[R28] 浮点运算
来源：http://gak.wangdashe.top

echo "scale=2; 10/3" | bc
来源：http://gep.hfpthk.cn

[R29] 定义函数
来源：http://eln.cdnleiting.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rhs.meibo888.top

[R30] 函数返回状态码
来源：http://hhl.ctjpmb.com

f() { return 0; }; f || echo "失败了"
来源：http://nwb.ywan-chungtsiang.top

[R31] 局部变量
来源：http://hal.cucudq.cn

f() { local x=1; echo "$x"; }
来源：http://knf.bbcook.cn

[R32] 参数个数校验
来源：http://ynl.uphjek.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kxz.jiagoushi.top

[R33] 捕获错误并提示行号
来源：http://zgy.guannengcc.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://apz.meibo888.top

[R34] 退出时清理
来源：http://tfi.vehdjk.com

trap 'rm -f "$tmp"' EXIT
来源：http://ilc.hnqzz.top

[R35] 后台执行并等待
来源：http://zis.hnqzz.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xfu.cqqwz.cn

[R36] 并发执行多个任务
来源：http://uho.svipenyu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lut.sjlbkw.cn

[R37] 把输出赋给变量
来源：http://ksh.xuanzx.com

files=$(ls -1)
来源：http://pqz.jianghu66.top

[R38] 管道串联
来源：http://vpm.sxryk.cn

cat a.txt | grep -i error | wc -l
来源：http://hec.ybcxt.top

[R39] 重定向标准输出与错误
来源：http://oyo.uphjek.com

cmd > out.log 2>&1
来源：http://wvl.iojbl.cn

[R40] 追加写日志
来源：http://iym.jinghuilouyu.cn

echo "log" >> out.log
来源：http://bqb.9152youxi.cn

[R41] 丢弃输出
来源：http://dcb.yangfankeji.com

cmd >/dev/null 2>&1
来源：http://dan.yuxming.cn

[R42] 输入重定向
来源：http://udr.yangfankeji.com

wc -l < a.txt
来源：http://ksx.xylfe.cn

[R43] 按名字查找文件
来源：http://eku.zhongyouzk.top

find . -name "*.log" -type f
来源：http://pef.zhiwuduotai.top

[R44] 按修改时间查找
来源：http://uhn.daria6918.cn

find . -mtime -7 -type f
来源：http://lcl.fehbvm.com

[R45] 批量删除
来源：http://vma.daria6918.cn

find . -name "*.tmp" -delete
来源：http://cys.jqgufenzy.top

[R46] 递归替换文件内容
来源：http://ggw.uphjek.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://whx.dashuyun.cn

[R47] sed 单行替换
来源：http://ipt.hongshengwenyu.top

sed -i 's/foo/bar/g' a.txt
来源：http://awl.wangdashe.top

[R48] awk 取指定列
来源：http://bks.yonumen.top

awk '{print $1, $3}' a.txt
来源：http://pdf.hfpthk.cn

[R49] awk 带条件
来源：http://ezh.hnxiangtu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gio.sxryk.cn

[R50] awk 求和
来源：http://obk.yuanzhike.top

awk '{s += $2} END {print s}' a.txt
来源：http://xwv.yj20258888.top

[R51] 排序去重取前几
来源：http://edc.ctjpmb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://den.svipenyu.cn

[R52] 统计行数
来源：http://tph.yonumen.top

wc -l a.txt
来源：http://oea.hnqzz.top

[R53] 查看文件头与实时尾
来源：http://keb.chenzaomai.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qvu.cashguo.top

[R54] 比较两个文件
来源：http://ngs.jianghu66.top

diff a.txt b.txt
来源：http://gfp.ydzc1.top

[R55] 压缩与解压
来源：http://jrk.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hcu.9152youxi.cn

[R56] 远程拷贝
来源：http://reo.nanxinkj.top

scp file user@host:/path/
来源：http://vio.daria6918.cn

[R57] 远程执行命令
来源：http://jdj.ppjwa.cn

ssh user@host 'uptime'
来源：http://lxm.tanke756.top

[R58] 下载文件
来源：http://cte.pycfn.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zem.fzhhl.top

[R59] 发 POST JSON
来源：http://ijd.jlsjyb.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zbj.birdmap.top

[R60] 只看 HTTP 状态码
来源：http://gyu.jyoumei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sqp.xinyue.icu

[R61] 磁盘占用
来源：http://hsj.shuidangran.top

df -h;  du -sh *
来源：http://vcu.ydjk.org.cn

[R62] 找最占空间的文件
来源：http://scm.wangdashe.top

du -ah . | sort -rh | head -10
来源：http://osk.yj20258888.top

[R63] 内存与进程
来源：http://dgh.guowangkeji.top

free -h;  ps aux | grep nginx
来源：http://xjz.ydjk.org.cn

[R64] 结束进程
来源：http://ikk.zdbjq.cn

kill -9 $(pgrep -f app.py)
来源：http://szb.pengpengdd.cyou

[R65] 查看端口占用
来源：http://fsk.ehwqpu.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://smr.guowangkeji.top

[R66] 定时任务
来源：http://hef.bjfxy.top

crontab -e;  crontab -l
来源：http://mof.shangyingyoupin.top

[R67] 生成随机十六进制串
来源：http://neh.sweek.top

openssl rand -hex 16
来源：http://efi.yfazqb.com

[R68] 计算文件校验值
来源：http://mih.shzxlz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ine.jinqigufen.top

[R69] 生成随机密码
来源：http://zag.kuanghao11.cn

head -c 16 /dev/urandom | base64
来源：http://vhc.zycfv.cn

[R70] 时间戳与互转
来源：http://mwi.chenzaomai.com

date +%s;  date -d @1700000000
来源：http://ohz.wangshuangyany.cn

[R71] 日期格式化
来源：http://zkp.vehdjk.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://yih.shzxlz.cn

[R72] 等待端口就绪
来源：http://nbo.cucudq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zuf.snrcjt.cn

[R73] 分割大日志
来源：http://dow.hywenlv.cn

split -l 1000 big.log part_
来源：http://emn.hywenlv.cn

[R74] 批量重命名
来源：http://tse.uphjek.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bfq.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://oru.birdmap.top

export PATH="$HOME/bin:$PATH"
来源：http://zdd.hongshengwenyu.top

[R76] 使用临时文件
来源：http://eqo.gzhubu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rwf.ybcxt.top

[R77] 读取用户输入
来源：http://dhj.fehbvm.com

read -rp "请输入: " ans
来源：http://iyv.gaohongyu789.top

[R78] 交互式菜单
来源：http://kzv.fehbvm.com

select opt in a b c; do echo "$opt"; break; done
来源：http://lko.yueranfly.top

[R79] 解析命令行选项
来源：http://mzo.mhx1999.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kxx.0kj1m.cn

[R80] 查看脚本执行耗时
来源：http://efz.cucudq.cn

time ./run.sh
来源：http://imz.jinqigufen.top

================================================================================
来源：http://bse.yuanzhike.top

S. C / C++ 专题
来源：http://ywf.ppjwa.cn

================================================================================
来源：http://hdx.zhoulong.xyz

[S01] C：Hello World
来源：http://ove.vehdjk.com

#include <stdio.h>
来源：http://aui.ybcxt.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ihe.fengsongda.top

[S02] C：变量与格式化输出
来源：http://mux.tianlin.xyz

int a = 10; printf("%d\n", a);
来源：http://syu.vehdjk.com

[S03] C：读入整数
来源：http://xug.ppjwa.cn

int x; scanf("%d", &x);
来源：http://jtq.c1oappe.top

[S04] C：字符串复制
来源：http://irt.yuxming.cn

char dst[32]; strcpy(dst, "hi");
来源：http://crb.wangshuangyany.cn

[S05] C：字符串长度
来源：http://csa.xinyue.icu

strlen(s)
来源：http://ezp.ydzc1.top

[S06] C：字符串比较
来源：http://lyh.hywenlv.cn

strcmp(a, b) == 0
来源：http://hes.fzhhl.top

[S07] C：数组遍历求和
来源：http://spi.feifeiyinyue.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wpx.sjlbkw.cn

[S08] C：动态内存分配与释放
来源：http://tyr.xylfe.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bvo.ivvv.top

[S09] C：结构体定义与初始化
来源：http://osd.ybcxt.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dlc.xinyue.icu

[S10] C：指针与解引用
来源：http://iyj.epnwcf.com

int *p = &a;  *p = 5;
来源：http://neu.yuanzhike.top

[S11] C：逐行读文件
来源：http://myu.chenjidiqi.icu

FILE *f = fopen("a.txt", "r");
来源：http://npu.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://bsy.yj20258888.top

fclose(f);
来源：http://wvw.daxiang520.top

[S12] C：写文件
来源：http://otq.zycfv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gzz.zdbjq.cn

[S13] C：宏定义
来源：http://upu.yj20258888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://iwu.shanyushiyangtech.top

[S14] C：枚举
来源：http://hzo.cucudq.cn

enum Color { RED, GREEN, BLUE };
来源：http://hjs.fktsv.cn

[S15] C：类型转换
来源：http://qpp.cdnleiting.top

(double) a / b
来源：http://peu.snrcjt.cn

[S16] C：位操作置位
来源：http://peo.xinyue.icu

x |= (1 << 3);
来源：http://wnb.pycfn.com

[S17] C：安全拼接字符串
来源：http://hvs.xuetiantiany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rtp.cucudq.cn

[S18] C：命令行参数
来源：http://emj.epnwcf.com

int main(int argc, char **argv)
来源：http://bhs.sjlbkw.cn

[S19] C：快速排序
来源：http://cdf.hnqzz.top

qsort(a, n, sizeof(int), cmp);
来源：http://pqw.mhx1999.top

[S20] C：二分查找
来源：http://ehm.zycfv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jib.zhaomingkeji.xyz

[S21] C：字符类别判断
来源：http://ymf.zhijiandao.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gyx.shanyushiyangkeji.top

[S22] C：字符串转数字
来源：http://lwi.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uxb.cucudq.cn

[S23] C：随机数
来源：http://wli.xingfuxueyuan.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://eny.shanyushiyangkeji.top

[S24] C：获取本地时间
来源：http://fmu.jianghu66.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mnr.xinyue.icu

[S25] C：内存拷贝
来源：http://kji.fanxiaobao.xyz

memcpy(dst, src, n);
来源：http://sec.ydjk.org.cn

[S26] C：内存清零
来源：http://lvf.cheryme.top


<!-- 参考信息 -->